Linear Independence – Lecture Notes

Definition:

Vectors  are linearly independent if the equation:



has only the trivial solution:



If other solutions exist, the vectors are linearly dependent.

Key Idea:

Independent vectors: No vector can be represented as a combination of the others.

Dependent vectors: At least one vector can be expressed as a linear combination of others.

Checking Linear Independence – Steps:

Form a matrix using vectors as columns.

Reduce matrix to Row-Echelon Form (REF).

If every column has a pivot, the vectors are independent.

If at least one column has no pivot (free variable), the vectors are dependent.

Examples:

Example 1: Independent Vectors

Check if vectors , , and  are independent.

Solution:

Form the matrix:
```cmatrix
| 1  0  0 |
| 0  1  0 |
| 0  0  1 |
```

The matrix is already in REF, with pivots in each column.

✅ Conclusion: Vectors are linearly independent.

Example 2: Dependent Vectors

Check if vectors  and  are independent.

Solution:

Form the matrix:

```
| 2  1 |
| 4  2 |
```

Apply row operation :

```
| 2  1 |
| 0  0 |
```

Second column has no pivot (free variable).

❌ Conclusion: Vectors are linearly dependent.

Reasoning: Vector , clearly dependent.

Example 3: Polynomials

Check independence of polynomials , , .

Solution:

Consider the equation:



Matching coefficients to zero polynomial gives:

Constant term: 

 term: 

 term: 

Only trivial solution exists.

 Conclusion: Polynomials are linearly independent.

Example 4: Functions

Check if  and  are linearly independent.

Solution:

Consider:



Test at two distinct points:





Thus, . Only trivial solution exists.

Conclusion: Functions are linearly independent.

Quick Tips:

Columns > Rows: Automatically dependent.

Zero Vector Included: Automatically dependent.

Set of two vectors: Dependent if they are scalar multiples.

Practical Importance:

Linear independence determines whether a set of vectors forms a basis for vector spaces, crucial in solving linear equations, spanning spaces, and dimension calculations.
