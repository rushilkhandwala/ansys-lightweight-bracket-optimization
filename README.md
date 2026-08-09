# Lightweight Cantilever Bracket Optimization in ANSYS

A first-year mechanical engineering FEA project studying how internal structures affect the mass, stress, deformation, factor of safety, and stiffness-to-weight ratio of a cantilever mounting bracket.

## Models Compared

1. Solid baseline
2. Uniform honeycomb lattice
3. Uniform triangular lattice
4. Hybrid triangular lattice

## Simulation Setup

- Material: Aluminum 6061-T6
- Analysis: Static Structural, ANSYS Mechanical
- Load: 490 N downward force
- Support: Rear mounting face fixed
- Mesh: 3 mm global mesh with local refinement at holes and internal cutout

## Final Results

| Model | Mass (g) | Max Deformation (mm) | Max Stress (MPa) | Factor of Safety |
|---|---:|---:|---:|---:|
| Solid | 694.90 | 0.00915 | 5.05 | 54.6 |
| Honeycomb | 591.39 | 0.01457 | 7.15 | 38.6 |
| Triangular | 626.71 | 0.01248 | 5.72 | 48.2 |
| Hybrid Triangular | 656.29 | 0.01131 | 4.88 | 56.5 |

## Conclusion

The hybrid triangular lattice achieved the lowest peak stress and highest factor of safety while using 5.6% less mass than the solid baseline. The solid model remained the stiffest, while the hybrid design provided the best strength-to-weight performance under the modeled loading condition.
