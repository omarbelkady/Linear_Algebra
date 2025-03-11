# Positive Definite Matrices  
## Key Concepts  
- **Definition**: \(A\) is positive definite if \(\mathbf{x}^T A \mathbf{x} > 0\) for all \(\mathbf{x} \neq 0\).  
- **Tests**:  
  - All eigenvalues > 0.  
  - Leading principal minors > 0 <button class="citation-flag" data-index="8">.  

## Example  
\(A = \begin{pmatrix} 2 & -1 \\ -1 & 2 \end{pmatrix}\) is positive definite (eigenvalues: 3, 1).  

## Applications  
- **Machine Learning**: Covariance matrices.  
- **Mechanics**: Energy functions.  

## Exercises  
1. Check if \(\begin{pmatrix} 1 & 2 \\ 2 & 1 \end{pmatrix}\) is positive definite.  
   **Solution**: No (eigenvalues: 3, -1).  