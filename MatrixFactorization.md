# Matrix Factorizations (LU, QR, Cholesky)

## Key Concepts

### **LU Decomposition**

The LU decomposition expresses a matrix as the product:

$$
A = LU
$$

where:
- `L` is a lower triangular matrix (with 1s on the diagonal in Doolittle's version)
- `U` is an upper triangular matrix

LU decomposition is useful for solving systems of equations using forward and backward substitution.

---

### **QR Decomposition**

The QR decomposition expresses a matrix as:

$$
A = QR
$$

where:
- `Q` is an orthogonal (or orthonormal) matrix, i.e., \( Q^T Q = I \)
- `R` is an upper triangular matrix

QR is often computed via the Gram-Schmidt process or Householder reflections. It's especially useful for solving least squares problems.

---

### **Cholesky Decomposition**

Used for symmetric, positive definite matrices:

$$
A = LL^T
$$

where:
- `L` is a lower triangular matrix
- `L^T` is its transpose

Cholesky is more efficient than LU for symmetric positive definite matrices and is widely used in optimization and statistics.

---

## Example: QR via Gram-Schmidt

Let:

$$
A = \begin{bmatrix}
1 & 1 \\
1 & 0 \\
1 & 1
\end{bmatrix}
$$
