# Applications to Differential Equations

## Key Concepts

- **Linear Systems**:

$$
\frac{d\mathbf{x}}{dt} = A\mathbf{x}
$$

- **Solution**:

$$
\mathbf{x}(t) = e^{At} \mathbf{x}_0
$$

where \( e^{At} \) is the matrix exponential.

## Example

For  

$$
A = \begin{pmatrix} 0 & 1 \\ -2 & -3 \end{pmatrix}
$$

1. **Eigenvalues**: \(-1\), \(-2\)

2. **General solution**:

$$
\mathbf{x}(t) = c_1 e^{-t}
\begin{pmatrix} 1 \\ -1 \end{pmatrix}
+
c_2 e^{-2t}
\begin{pmatrix} 1 \\ -2 \end{pmatrix}
$$

## Applications

- **Engineering**: Circuit analysis  
- **Biology**: Population dynamics

## Exercises

1. Solve  

$$
\frac{dx}{dt} = 3x,\quad x(0) = 2
$$  

**Solution**:  

$$
x(t) = 2e^{3t}
$$
