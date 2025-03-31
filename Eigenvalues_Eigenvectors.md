# 4. Eigenvalues and Eigenvectors

## 4.1 Key Concepts

- **Definition**:  
  For a square matrix \( A \), \( \lambda \) is an eigenvalue and \( \mathbf{v} \) is an eigenvector if:

$$
A\mathbf{v} = \lambda \mathbf{v}
$$

- **Characteristic Equation**:

$$
\det(A - \lambda I) = 0
$$

## 4.2 Properties
- Eigenvectors corresponding to distinct eigenvalues are linearly independent
- **Trace** = Sum of eigenvalues
- **Determinant** = Product of eigenvalues

## 4.3 Example
**Problem**: Find eigenvalues of

$$
A = \begin{bmatrix} 4 & 1 \\ 2 & 3 \end{bmatrix}
$$

1. Solve the characteristic equation:

$$
\det\begin{bmatrix} 4-\lambda & 1 \\ 2 & 3-\lambda \end{bmatrix} = (4-\lambda)(3-\lambda) - 2 = \lambda^2 - 7\lambda + 10 = 0
$$

2. Eigenvalues:

$$
\lambda_1 = 5, \lambda_2 = 2
$$

---

## 4.4 Applications
- **Principal Component Analysis (PCA)**: Dimensionality reduction in data science
- **Quantum Mechanics**: Energy levels of quantum systems

## 4.5 Exercises
1. Find eigenvalues of

$$
B = \begin{bmatrix} 2 & 7 \\ -1 & -6 \end{bmatrix}
$$  

**Solution**:

$$
\lambda = -5, 1
$$
