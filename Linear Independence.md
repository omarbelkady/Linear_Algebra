
# Linear Independence – Lecture Notes

## Definition:

Vectors \( \mathbf{v}_1, \mathbf{v}_2, \dots, \mathbf{v}_n \) are **linearly independent** if the equation:

\[
c_1 \mathbf{v}_1 + c_2 \mathbf{v}_2 + \dots + c_n \mathbf{v}_n = \mathbf{0}
\]

has only the **trivial solution**:

\[
c_1 = c_2 = \dots = c_n = 0
\]

If other solutions exist, the vectors are **linearly dependent**.

---

## Key Idea:

- **Independent** vectors: No vector can be represented as a combination of the others.
- **Dependent** vectors: At least one vector can be expressed as a linear combination of others.

---

## Checking Linear Independence – Steps:

1. Form a matrix using vectors as columns.
2. Reduce matrix to Row-Echelon Form (REF).
3. If every column has a pivot, the vectors are independent.
4. If at least one column has no pivot (free variable), the vectors are dependent.

---

## Examples:

### Example 1: Independent Vectors

Check if vectors \(\mathbf{u}=(1, 0, 0)\), \(\mathbf{v}=(0, 1, 0)\), and \(\mathbf{w}=(0, 0, 1)\) are independent.

**Solution**:

Form the matrix:
\[
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
\]

The matrix is already in **REF**, with pivots in each column.

✅ **Conclusion**: Vectors are **linearly independent**.

---

### Example 2: Dependent Vectors

Check if vectors \(\mathbf{a}=(2, 4)\) and \(\mathbf{b}=(1, 2)\) are independent.

**Solution**:

Form the matrix:
\[
\begin{bmatrix}
2 & 1 \\
4 & 2
\end{bmatrix}
\xrightarrow{R_2 \to R_2 - 2R_1}
\begin{bmatrix}
2 & 1 \\
0 & 0
\end{bmatrix}
\]

Second column has no pivot (free variable).

❌ **Conclusion**: Vectors are **linearly dependent**.

Reasoning: Vector \(\mathbf{a}=2\mathbf{b}\), clearly dependent.

---

### Example 3: Polynomials

Check independence of polynomials \(1\), \(x\), \(x^2\).

**Solution**:

Consider the equation:
\[
c_1(1) + c_2(x) + c_3(x^2) = 0
\]

Matching coefficients to zero polynomial gives:

- Constant term: \(c_1=0\)
- \(x\) term: \(c_2=0\)
- \(x^2\) term: \(c_3=0\)

Only trivial solution exists.

✅ **Conclusion**: Polynomials are **linearly independent**.

---

### Example 4: Functions

Check if \( e^x \) and \( e^{3x} \) are linearly independent.

**Solution**:

Consider:
\[
c_1 e^x + c_2 e^{3x} = 0 \quad \text{for all } x
\]

Test at two distinct points:

- \(x=0:\quad c_1 + c_2=0\Rightarrow c_1=-c_2\)
- \(x=1:\quad c_1 e + c_2 e^3=0\Rightarrow -c_2 e + c_2 e^3=0\Rightarrow c_2(e^3 - e)=0\Rightarrow c_2=0\)

Thus, \( c_1=0 \). Only trivial solution exists.

✅ **Conclusion**: Functions are **linearly independent**.

---

## Quick Tips:

- **Columns > Rows**: Automatically dependent.
- **Zero Vector Included**: Automatically dependent.
- **Set of two vectors**: Dependent if they are scalar multiples.

---

## Practical Importance:

Linear independence determines whether a set of vectors forms a **basis** for vector spaces, crucial in solving linear equations, spanning spaces, and dimension calculations.
