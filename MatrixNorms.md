# Matrix Norms  
## Key Concepts  
- **Frobenius Norm**: \(\|A\|_F = \sqrt{\sum_{i,j} |a_{ij}|^2}\).  
- **Operator Norm**: \(\|A\| = \max_{\|\mathbf{x}\|=1} \|A\mathbf{x}\|\) <button class="citation-flag" data-index="8">.  

## Example  
For \(A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}\):  
- \(\|A\|_F = \sqrt{1 + 4 + 9 + 16} = \sqrt{30}\).  

## Applications  
- **Machine Learning**: Regularization (e.g., L2 penalty).  
- **Control Theory**: System stability analysis.  

## Exercises  
1. Compute \(\|A\|_F\) for \(A = \begin{pmatrix} 0 & 1 \\ -1 & 0 \end{pmatrix}\).  
   **Solution**: \(\sqrt{2}\).  