# Corrected 2025 Reverification Update

Author: Tadashi Mazusaki  
Status: Corrected post-invalidation research dataset / preliminary analysis  
Zenodo DOI: https://doi.org/10.5281/zenodo.20510158  
Publication date: 2026-06-02

## Summary

This note records the corrected 2025 reverification update for the Da-P / DICP 3D asymmetric model.

The dataset was published after the prior invalidation of earlier numerical claims. It should be cited as a corrected post-invalidation research dataset and preliminary analysis, not as final proof of a new universality class.

## Corrected Dataset

Three high-statistics single-size simulations were included:

| L | Runs | Steps | Peak p* | chi_max |
|---|------|-------|---------|---------|
| 80 | 500 | 20000 | 0.031225 | 9908.2 |
| 96 | 500 | 20000 | 0.029465 | 16975.7 |
| 128 | 500 | 20000 | 0.026650 | 39906.5 |

The corrected data show candidate anomalous susceptibility finite-size scaling:

```text
chi_max ~ L^(gamma/nu)
gamma/nu ~= 2.965
R^2 ~= 0.999997
```

## Interpretation

The exponent estimate is robust across the three available system sizes for the measured susceptibility peaks. However, estimates of `p_c(infinity)` and `nu` remain unstable with only three system sizes.

The result should therefore be described as:

```text
candidate anomalous finite-size scaling behavior
```

not as:

```text
confirmed new universality class
```

## Relation to Prior Invalidation

The previous invalidation record is:

https://doi.org/10.5281/zenodo.16780090

That record invalidated earlier numerical claims affected by a flaw in the original simulation rules. The corrected 2025 reverification dataset is intended to document the subsequent corrected numerical work.

## Recommended Next Validation Steps

Future work should include:

1. Additional system sizes, especially smaller and larger L values.
2. Bootstrap or jackknife uncertainty estimates.
3. Independent implementation checks.
4. Comparison of peak extraction methods.
5. Clear separation of raw, survival-conditioned, and corrected susceptibility observables.

## Citation

Mazusaki, T. (2026). Corrected 2025 Reverification Results for the Da-P/DICP 3D Asymmetric Model: Candidate Anomalous Finite-Size Scaling. Zenodo. https://doi.org/10.5281/zenodo.20510158
