# **3. Determinants**

## **3.1 Definition and Properties**
The determinant of a square matrix $ A $ measures the scaling factor of the transformation represented by $ A $.

### Example 1:
For a $ 2 \times 2 $ matrix:
A =
\begin{bmatrix}
a & b \
c & d
\end{bmatrix},

thedeterminantis:
\det(A) = ad - bc.

Example:
A =
\begin{bmatrix}
1 & 2 \
3 & 4
\end{bmatrix},
\quad \det(A) = (1)(4) - (2)(3) = -2.


---

## **3.2 Computation of Determinants**
### Cofactor Expansion
For larger matrices, use cofactor expansion along a row or column.

#### Example 1:
Compute the determinant of:
A =
\begin{bmatrix}
1 & 2 & 3 \
0 & 4 & 5 \
1 & 0 & 6
\end{bmatrix}.

Expandalongthefirstrow:
\det(A) = 1 \cdot \det\begin{bmatrix} 4 & 5 \ 0 & 6 \end{bmatrix}

2 \cdot \det\begin{bmatrix} 0 & 5 \ 1 & 6 \end{bmatrix}
3 \cdot \det\begin{bmatrix} 0 & 4 \ 1 & 0 \end{bmatrix}.
$$
Compute minors:

det(A)=1(24−0)−2(0−5)+3(0−4)=24+10−12=22.
