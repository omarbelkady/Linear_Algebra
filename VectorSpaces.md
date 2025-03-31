# **2. Vector Spaces**

## **2.1 Definition and Properties**
A vector space is a set of objects (vectors) that can be added and scaled while satisfying certain axioms.

### Example 1:
The set 

$$
\mathbb{R}^2
$$ 

with standard addition and scalar multiplication forms a vector space.

### Example 2:
The set of all polynomials of degree $$ \leq 2 $$ denoted $$ P_2 $$ is a vector space:

$$
P_2 = \{a_0 + a_1x + a_2x^2 \mid a_0, a_1, a_2 \in \mathbb{R}\}
$$

---

## **2.2 Subspaces**

A subspace is a subset of a vector space that is itself a vector space.

### Example 1:

In 

$$
\mathbb{R}^3
$$

the xy-plane 

$$
\{(x, y, 0) \mid x, y \in \mathbb{R}\} 
$$ 

is a subspace.

### Example 2:

The null space of a matrix $$ A $$ is a subspace. For example, if:

$$
A = \begin{bmatrix} 1 & 2 \\ 2 & 4 \end{bmatrix}
$$

the null space is

$$
\{(x, y) \mid x + 2y = 0\}
$$

---

## **2.3 Row Space**

### Definition

The row space of a matrix $$ A $$ is the subspace spanned by its rows. It is a subspace of

$$
\mathbb{R}^n
$$ 

if

$$
A
$$ 

is an

$$
m \times n
$$

matrix

### Example 1:

Let:

$$ 
A = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}
$$

The rows are:

$$
\mathbf{r}_1 = \begin{bmatrix} 1 & 2 & 3 \end{bmatrix}, \mathbf{r}_2 = \begin{bmatrix} 4 & 5 & 6 \end{bmatrix}
$$

The row space is:

$$
\text{Row Space}(A) = \text{span}\{\mathbf{r}_1, \mathbf{r}_2\}
$$

### Finding the Row Space

Perform row reduction to find a basis for the row space.

### Example 2:

Reduce 

$$ A $$ 

to row echelon form:

$$
A = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end {bmatrix} \xrightarrow{R_2 \to R_2 - 4R_1} \begin {bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end {bmatrix}
$$

The nonzero rows of the reduced matrix form a basis for the row space:

$$
\text{Basis} = \left\lbrace
\begin{array}{c} 1 \\ 2 \\ 3 \end{array},
\begin{array}{c} 0 \\ -3 \\ -6 \end{array}
\right\rbrace
$$

## **2.4 Null Space**

### Definition

The null space (or kernel) of a matrix

$$
A
$$ 

is the set of all vectors $$ \mathbf{x} $$ such that:

$$
A\mathbf{x} = \mathbf{0}
$$

### Example 1:

Let:

$$
A = \begin{bmatrix} 1 & 2 \\ 2 & 4 \end{bmatrix}
$$

Solve

$$
A\mathbf{x} = \mathbf{0}
$$

$$ 
\begin{bmatrix} 1 & 2 \\ 2 & 4 \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \end{bmatrix}
$$

Row reduce:

$$
\begin{bmatrix} 1 & 2 \\ 2 & 4 \end{bmatrix} \xrightarrow{R_2 \to R_2 - 2R_1} \begin{bmatrix} 1 & 2 \\ 0 & 0 \end{bmatrix} 
$$

The solution is:

$$
x_1 + 2x_2 = 0 \implies x_1 = -2x_2
$$

Thus:

$$
\text{Basis} = \left \lbrace \begin{bmatrix} 1 \\ 3 \\ 5 \end{bmatrix}, \begin{bmatrix} 2 \\ 4 \\ 6 \end{bmatrix} \right\rbrace
$$

### Properties

- The null space is always a subspace
- Its dimension is called the **nullity** of $$ A $$



## **2.5 Column Space**

### Definition

The column space of a matrix $$ A $$ is the subspace spanned by its columns. It is a subspace of 

$$
\mathbb{R}^m
$$

if 

$$ 
A 
$$ 

is an

$$
m \times n
$$

matrix.

### Example 1:

Let:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \\ 5 & 6 \end{bmatrix}
$$

The columns are:

$$
\mathbf{c}_1 = \begin{bmatrix} 1 \\ 3 \\ 5 \end{bmatrix}, \mathbf{c}_2 = \begin{bmatrix} 2 \\ 4 \\ 6 \end{bmatrix}
$$

The column space is:

$$
\text{Column Space}(A) = \text{span}\{\mathbf{c}_1, \mathbf{c}_2\}
$$

### Finding the Column Space

Perform row reduction to identify pivot columns, which form a basis for the column space.

### Example 2:

Reduce 

$$
A 
$$ 

to row echelon form:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \\ 5 & 6 \end{bmatrix} \xrightarrow{R_2 \to R_2 - 3R_1, R_3 \to R_3 - 5R_1} \begin{bmatrix} 1 & 2 \\ 0 & -2 \\ 0 & -4 \end{bmatrix}
$$

Further reduce:

$$
\begin{bmatrix} 1 & 2 \\ 0 & -2 \\ 0 & -4 \end{bmatrix} \xrightarrow{R_3 \to R_3 - 2R_2} \begin{bmatrix} 1 & 2 \\ 0 & -2 \\ 0 & 0 \end{bmatrix}
$$

The pivot columns are the first two columns of $$ A $$. 

Thus:

$$
\text{Basis} = \left\langle \begin{bmatrix} 1 \\ 3 \\ 5 \end{bmatrix}, \begin{bmatrix} 2 \\ 4 \\ 6 \end{bmatrix} \right\rangle
$$
