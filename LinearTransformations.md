# Linear Transformations and Change of Basis

## Key Concepts

- **Definition**: A function `T: Rⁿ → Rᵐ` is linear if:
  - `T(u + v) = T(u) + T(v)`
  - `T(c * v) = c * T(v)`

## Change of Basis

- **Coordinate Vector**:  
  `[v]_B = (c₁, ..., cₙ)^T` where `v = c₁ * b₁ + ... + cₙ * bₙ`

- **Transformation Matrix**:  
  `A_B = P⁻¹ A P`  
  where `P` is the change-of-basis matrix

## Example

**Problem**: Find `T(x) = [[2, 1], [1, 2]] * x` in basis `B = {(1,1), (1,-1)}`

1. Compute `P = [[1, 1], [1, -1]]`
2. Then `A_B = P⁻¹ A P = [[3, 0], [0, 1]]`

## Applications

- **Computer Graphics**: Coordinate system transformations
- **Quantum Mechanics**: Basis changes for wavefunctions

## Exercises

1. Find `A_B` for `A = [[1, 2], [3, 4]]` and `B = {(2,1), (1,1)}`
   - **Solution**: `A_B = [[8, 5], [-5, -2]]`
