# Inner Product Spaces

## Key Concepts

- **Inner Product**: Generalizes the dot product:  
  `<u, v>` satisfies linearity and symmetry.

- **Induced Norm**:  
  `||u|| = sqrt(<u, u>)`

---

## Example

In P₂ (polynomials of degree ≤ 2):  
`<p, q> = ∫_{-1}^1 p(x)q(x) dx`

---

## Exercises

1. Compute `<x², x+1>` in P₂:

<x², x+1> = ∫{-1}^1 x²(x+1) dx
= ∫{-1}^1 (x³ + x²) dx
= ∫{-1}^1 x³ dx + ∫{-1}^1 x² dx
= 0 (x³ is odd) + 2∫₀¹ x² dx
= 2 * [x³ / 3]₀¹
= 2/3


Final Answer: `2/3`
