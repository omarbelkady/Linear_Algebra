# Linear Transformations and Change of Basis  
## Key Concepts  
- **Definition**: A function \(T: \mathbb{R}^n \to \mathbb{R}^m\) is linear if:  
  - \(T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})\)  
  - \(T(c\mathbf{v}) = cT(\mathbf{v})\) <button class="citation-flag" data-index="4">.  

## Change of Basis  
- **Coordinate Vector**:  
  \([\mathbf{v}]_{\mathcal{B}} = \begin{pmatrix} c_1 \\ \vdots \\ c_n \end{pmatrix}\) for \(\mathbf{v} = c_1 \mathbf{b}_1 + \dots + c_n \mathbf{b}_n\).  
- **Transformation Matrix**:  
  \[
  A_{\mathcal{B}} = P^{-1} A P
  \]  
  where \(P\) is the change-of-basis matrix <button class="citation-flag" data-index="6">.  

## Example  
**Problem**: Find \(T(\mathbf{x}) = \begin{pmatrix} 2 & 1 \\ 1 & 2 \end{pmatrix}\mathbf{x}\) in basis \(\mathcal{B} = \{(1, 1), (1, -1)\}\).  
1. Compute \(P = \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}\).  
2. \(A_{\mathcal{B}} = P^{-1} A P = \begin{pmatrix} 3 & 0 \\ 0 & 1 \end{pmatrix}\).  

## Applications  
- **Computer Graphics**: Coordinate system transformations.  
- **Quantum Mechanics**: Basis changes for wavefunctions <button class="citation-flag" data-index="6">.  

## Exercises  
1. Find \(A_{\mathcal{B}}\) for \(A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}\) and \(\mathcal{B} = \{(2, 1), (1, 1)\}\).  
   **Solution**: \(A_{\mathcal{B}} = \begin{pmatrix} 8 & 5 \\ -5 & -2 \end{pmatrix}\).  