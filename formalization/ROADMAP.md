# Formalization roadmap

## Goal

Develop a machine-checked account of the exact binary quadratic theory first,
then extend the library toward the ternary and general-alphabet results where
the required analytic infrastructure is available.

## Design decisions still open

- Proof assistant and pinned version (Lean 4 with mathlib is the leading option,
  but is not yet fixed).
- Representation of finitely supported functions and finite product alphabets.
- Whether convolution is developed first on finite groups, on `Z^d`, or through
  a reusable finitely-supported abstraction.
- Treatment of real, nonnegative, and complex-valued equality cases.

## Proposed milestones

1. **Foundations**
   - Finite product alphabets and counting-measure `l^p` norms.
   - Finitely supported convolution and reflection.
   - Tensor products and coordinate slicing.
2. **Exact tensorization**
   - One-coordinate best constants.
   - Product upper and lower bounds.
   - Equality propagation across coordinates.
3. **Binary quadratic reduction**
   - Two-point parametrization.
   - Hilbertian identity at output exponent `r = 2`.
   - Boundary reduction of the optimization problem.
4. **One-variable phase diagram**
   - Definition and basic properties of the boundary function.
   - Constant-one exponent region.
   - Sharpness and equality cases.
5. **Consequences**
   - Cross-additive energy and sumset formulations.
   - Entropy and Fourier formulations.
6. **Later extensions**
   - Ternary two-envelope mechanism.
   - Reflection structure for general alphabets.
   - Parity renormalization and the discrete-continuous bridge.

## Traceability convention

Every formal theorem should record the corresponding LaTeX label from
`paper/main.tex` in a nearby comment. A future theorem index should map each
paper label to its formal source file and report one of: `planned`, `partial`,
or `complete`.
