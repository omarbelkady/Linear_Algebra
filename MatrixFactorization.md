# Matrix Factorizations (LU, QR, Cholesky)  
## Key Concepts  
- **LU Decomposition**: \(A = LU\) (lower-upper triangular) <button class="citation-flag" data-index="8">.  
- **QR Decomposition**: \(A = QR\) (orthogonal \(Q\), upper triangular \(R\)).  
- **Cholesky Decomposition**: \(A = LL^T\) for symmetric positive definite \(A\).  

## Example: QR via Gram-Schmidt  
For \(A = \begin{pmatrix} 1 & 1 \\ 1 & 0 \\ 1 & 1 \end{pmatrix}\):  
1. Orthogonalize columns to get \(Q\).  
2. \(R = Q^T A\).  

## Applications  
- **Numerical Solvers**: LU for solving \(A\mathbf{x} = \mathbf{b}\).  
- **Optimization**: Cholesky in quadratic programming.  

## Exercises  
1. Compute Cholesky decomposition of \(\begin{pmatrix} 4 & 2 \\ 2 & 10 \end{pmatrix}\).  
   **Solution**: \(L = \begin{pmatrix} 2 & 0 \\ 1 & 3 \end{pmatrix}\).  