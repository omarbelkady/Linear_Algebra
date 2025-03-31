# Least Squares Approximation

## Key Concepts
- **Problem Statement**:  
  Solve the overdetermined system

$$
A\mathbf{x} \approx \mathbf{b}
$$

  where

$$
A \in \mathbb{R}^{m \times n}
$$

  with

$$
m > n
$$

- **Normal Equations**:  

$$
A^T A \mathbf{x} = A^T \mathbf{b}
$$
  
  The solution minimizes

$$
\|A\mathbf{x} - \mathbf{b}\|^2
$$

## Derivation Methods
1. **Calculus Approach**:

- Differentiate

$$ 
\|A\mathbf{x} - \mathbf{b}\|^2 $$ w.r.t. $$ \mathbf{x} 
$$

- Set gradient to zero to obtain normal equations

2. **Projection Approach**:

- Find

$$
\mathbf{x}
$$

such that

$$
A\mathbf{x}
$$

is the orthogonal projection of

$$
\mathbf{b}
$$

onto

$$
\text{Col}(A)
$$

## Examples

### Example 1: Line Fitting

Fit 

$$
y = mx + b
$$

to points

$$
(1, 2)
$$

$$
(2, 2)
$$

$$
(3, 4)
$$

1. Construct system:

$$
A = \begin{bmatrix}
1 & 1 \\
1 & 2 \\ 
1 & 3
\end{bmatrix}, \quad
\mathbf{b} = \begin{bmatrix}
2 \\
2 \\
4
\end{bmatrix}
$$

3. Solve normal equations:
 
$$
A^T A = \begin{bmatrix}
3 & 6 \\
6 & 14
\end{bmatrix}, \quad
A^T \mathbf{b} = \begin{bmatrix}
8 \\
18
\end{bmatrix}
$$
   
Solution:

$$
m = 1
$$

$$
b = 1
$$

### Example 2: Quadratic Fit
Fit

$$
y = ax^2 + bx + c
$$

to

$$
(0,1)
$$

$$ 
(1,3)
$$

$$
(2,7)
$$

$$
(3,13)
$$

1. Design matrix:

$$
A = \begin{bmatrix}
1 & 0 & 0 \\
1 & 1 & 1 \\
1 & 2 & 4 \\
1 & 3 & 9
\end{bmatrix}
$$

2. Solution yields:

$$
a = 1 
$$

$$
b = 1
$$

$$
c = 1
$$

## Applications
- **Statistics**: Linear regression models
- **Signal Processing**: Filter design
- **Computer Vision**: Camera calibration
- **Control Systems**: Optimal state estimation

## Exercises

### Exercise 1

Solve:

$$
\begin{bmatrix}
1 & 0 \\
1 & 1 \\
1 & 2
\end{bmatrix}
\mathbf{x} = 
\begin{bmatrix}
1 \\
3 \\
4
\end{bmatrix}
$$

**Solution**:

$$
\mathbf{x} = \begin{bmatrix}
0.5 \\
2.25
\end{bmatrix}
$$

### Exercise 2
Find the least squares line for 

$$
(-1,1)
$$

$$
(0,0)
$$

$$
(1,1)
$$

$$ 
(2,4)
$$

**Solution**:

$$
y = 1.1x + 0.1
$$

## Implementation (Python)

```python
import numpy as np
A = np.array([[1,1], [1,2], [1,3]])
b = np.array([2, 2, 4])
x = np.linalg.lstsq(A, b, rcond=None)[0]
```
