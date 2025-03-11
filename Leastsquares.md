# Least Squares Approximation  
## Key Concepts  
- **Problem**: Solve \(A\mathbf{x} \approx \mathbf{b}\) when \(A\) is tall (\(m > n\)).  
- **Normal Equations**: \(A^T A \mathbf{x} = A^T \mathbf{b}\) <button class="citation-flag" data-index="4">.  

## Derivation  
Minimize \(\|A\mathbf{x} - \mathbf{b}\|^2\) using calculus or projections.  

## Example  
Fit a line \(y = mx + b\) to points \((1, 2)\), \((2, 2)\), \((3, 4)\):  
1. \(A = \begin{pmatrix} 1 & 1 \\ 1 & 2 \\ 1 & 3 \end{pmatrix}\), \(\mathbf{b} = \begin{pmatrix} 2 \\ 2 \\ 4 \end{pmatrix}\).  
2. Solve \(A^T A \mathbf{x} = A^T \mathbf{b}\) to get \(m = 1\), \(b = 1\).  

## Applications  
- **Regression**: Linear models in statistics.  
- **Control Theory**: Optimal control inputs.  

## Exercises  
1. Solve \( \begin{pmatrix} 1 & 0 \\ 1 & 1 \\ 1 & 2 \end{pmatrix} \mathbf{x} = \begin{pmatrix} 1 \\ 3 \\ 4 \end{pmatrix} \).  
   **Solution**: \(\mathbf{x} = (0.5, 2.25)\).  