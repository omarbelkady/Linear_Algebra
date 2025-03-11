# Eigenvalues and Eigenvectors  
## Key Concepts  
- **Definition**:  
  For a square matrix \(A\), \(\lambda\) is an eigenvalue and \(\mathbf{v}\) is an eigenvector if:  
  \[
  A\mathbf{v} = \lambda \mathbf{v}
  \]  
- **Characteristic Equation**:  
  \[
  \det(A - \lambda I) = 0
  \] <button class="citation-flag" data-index="4"><button class="citation-flag" data-index="6">.  

## Properties  
- Eigenvectors of distinct eigenvalues are linearly independent.  
- Trace = Sum of eigenvalues, Determinant = Product of eigenvalues.  

## Example  
**Problem**: Find eigenvalues of \(A = \begin{pmatrix} 4 & 1 \\ 2 & 3 \end{pmatrix}\).  
1. Characteristic equation:  
   \[
   \det\left(\begin{pmatrix} 4-\lambda & 1 \\ 2 & 3-\lambda \end{pmatrix}\right) = \lambda^2 - 7\lambda + 10 = 0
   \]  
   Roots: \(\lambda_1 = 5\), \(\lambda_2 = 2\).  

## Applications  
- **PCA**: Dimensionality reduction in data science <button class="citation-flag" data-index="4">.  
- **Quantum Mechanics**: Energy levels of particles <button class="citation-flag" data-index="6">.  

## Exercises  
1. Find eigenvalues of \(B = \begin{pmatrix} 2 & 7 \\ -1 & -6 \end{pmatrix}\).  
   **Solution**: \(\lambda = -5, 1\).  