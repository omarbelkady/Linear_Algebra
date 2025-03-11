# Orthogonalization and Gram-Schmidt Process  
## Key Concepts  
- **Orthogonal Sets**: Vectors \(\mathbf{u}_1, \dots, \mathbf{u}_n\) are orthogonal if \(\mathbf{u}_i \cdot \mathbf{u}_j = 0\) for \(i \neq j\).  
- **Gram-Schmidt Process**: Converts a basis into an orthogonal/orthonormal basis <button class="citation-flag" data-index="8">.  

## Algorithm  
Given basis \(\{\mathbf{v}_1, \dots, \mathbf{v}_n\}\):  
1. \(\mathbf{u}_1 = \mathbf{v}_1\).  
2. \(\mathbf{u}_k = \mathbf{v}_k - \sum_{i=1}^{k-1} \frac{\mathbf{v}_k \cdot \mathbf{u}_i}{\|\mathbf{u}_i\|^2} \mathbf{u}_i\).  

## Example  
Orthogonalize \(\{(1, 1, 1), (1, 0, 1), (0, 1, 2)\}\):  
1. \(\mathbf{u}_1 = (1, 1, 1)\).  
2. \(\mathbf{u}_2 = (1, 0, 1) - \frac{2}{3}(1, 1, 1) = (\frac{1}{3}, -\frac{2}{3}, \frac{1}{3})\).  

## Applications  
- **QR Decomposition**: Factor \(A = QR\) using orthogonalization <button class="citation-flag" data-index="8">.  
- **Signal Processing**: Orthogonal basis functions (e.g., Fourier series).  

## Exercises  
1. Orthogonalize \(\{(2, 0), (3, 1)\}\).  
   **Solution**: \(\{(2, 0), (0, 1)\}\).  