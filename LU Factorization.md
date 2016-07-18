* A = LU Factorization
    The goal of the factorization is to find the matrix L so that A = LU.

    The inverse of the matrix product AB is B^-1 * A^-1

    Transpose matrix is a matrix with its rows and columns exchanged. So (A^t)ij = Aji. And like inverse the transpose of a matrix product AB is B^tA^t. And likewise inverse of A^t is (A^-1)^t.

    The basic idea of LU factorization is to move the elimination matrix E21 * E31...A = U from the left of the equality sign to the right side. This can be done by multiplying each of the elimination matrix by their inverse in reverse order to produce the I matrix, and the product of those inverse matrices is the L in A = LU, L stands for lower triangular form.

    It is possible that sometimes we wish to strip out the diagonal pivots and create the A = LDU form of A.

    Another reason why we prefer L over E is that the combination of row subtractions does not have the same effect on L that it does on E (so it's much cleaner).

* Cost of Elimination
    Cost of inverting matrix size n is about 1/3 N ^ 3. (price of elimination)

* Row exchange
    There are about n! ways to create a permutation matrix. The inverse and transpose of a permutation matrix is the same p^t

* From Book
    Multipliers of the L are exactly the multipliers lij, multiplying pivot row j when it was subtracted from row i.

    One of the best things about L in LU factorization is that each Lij goes directly to it's ij position in the inverse product L, without taking into account the usual mixup that results from matrix multiplications.

    Assuming no row exchanges, anytime row or column of A starts with 0, the same row/column of l also starts with 0.
