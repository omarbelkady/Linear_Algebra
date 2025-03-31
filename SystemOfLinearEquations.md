1. Systems of Linear Equations
1.1 Introduction
A system of linear equations consists of multiple linear equations involving the same set of variables. The goal is to find values for the variables that satisfy all equations simultaneously.

Example 1:
x+2y
3x−y
​
  
=5,
=1.
​
 
This system can be written in matrix form as:
$$
\begin{bmatrix}
1 & 2 \
3 & -1
\end{bmatrix}
\begin{bmatrix}
x \ y
\end{bmatrix}
\begin{bmatrix}
5 \ 1
\end{bmatrix}.


### Example 2:
\begin{aligned}
x_1 + x_2 + x_3 &= 6, \
2x_1 - x_2 + 3x_3 &= 14, \
x_1 + 2x_2 - x_3 &= -2.
\end{aligned}

Matrixform:
\begin{bmatrix}
1 & 1 & 1 \
2 & -1 & 3 \
1 & 2 & -1
\end{bmatrix}
\begin{bmatrix}
x_1 \ x_2 \ x_3
\end{bmatrix}
\begin{bmatrix}
6 \ 14 \ -2
\end{bmatrix}.


---

## **1.2 Solving Systems of Linear Equations**
### Gaussian Elimination
Gaussian elimination reduces a system to row echelon form (REF) or reduced row echelon form (RREF).

#### Example 1:
Solve:
\begin{aligned}
x + 2y &= 5, \
3x - y &= 1.
\end{aligned}

Augmentedmatrix:
\begin{bmatrix}
1 & 2 & | & 5 \
3 & -1 & | & 1
\end{bmatrix}.


Perform row operations:
1. $ R_2 \to R_2 - 3R_1 $:
\begin{bmatrix}
1 & 2 & | & 5 \
0 & -7 & | & -14
\end{bmatrix}.

2. Normalize $ R_2 $: $ R_2 \to R_2 / -7 $:
\begin{bmatrix}
1 & 2 & | & 5 \
0 & 1 & | & 2
\end{bmatrix}.

3. Back substitution: $ y = 2 $, $ x + 2(2) = 5 \implies x = 1 $.

Solution: $ x = 1, y = 2 $.