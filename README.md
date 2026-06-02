# Da-P Particle Theory (DICP)

## Planck-Continuous Cosmos Hypothesis

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

Da-P Particle Theory proposes a theoretical framework in which spacetime is modeled as a network of Planck-scale information-cohesion cells bound by Dimensional Information Cohesion Particles (DICP, Da-P particles). The framework is currently a working hypothesis under active revision.

This repository collects background documents, corrected numerical notes, and theoretical extensions of the Da-P / DICP framework.

---

## 2026 Update: Corrected Reverification and Cosmological Residual Hypothesis

Two new Zenodo records were published on 2026-06-02:

| Record | DOI | Local note |
|--------|-----|------------|
| Corrected 2025 reverification dataset for the Da-P / DICP 3D asymmetric model | https://doi.org/10.5281/zenodo.20510158 | [docs/DaP_2025_Reverification_Update.md](docs/DaP_2025_Reverification_Update.md) |
| Da-P Cosmological Constant Residual Hypothesis | https://doi.org/10.5281/zenodo.20510743 | [docs/DaP_Cosmological_Constant_Residual_Hypothesis.md](docs/DaP_Cosmological_Constant_Residual_Hypothesis.md) |

Important status note:

- Earlier numerical claims were invalidated in the prior Zenodo record: https://doi.org/10.5281/zenodo.16780090
- The corrected 2025 reverification dataset should be treated as a post-invalidation research dataset and preliminary analysis.
- The current finite-size scaling result is a candidate anomalous scaling behavior, not final proof of a new universality class.
- The cosmological constant residual hypothesis is a theoretical reformulation and does not claim to solve the cosmological constant problem.

---

## Published Background Documents

### Background Documents (v1.0 - October 2025)

| Language | Audience | DOI | PDF |
|----------|----------|-----|-----|
| Japanese | General | [10.5281/zenodo.17244161](https://doi.org/10.5281/zenodo.17244161) | [Download](https://zenodo.org/records/17244161) |
| English | General | [10.5281/zenodo.17244360](https://doi.org/10.5281/zenodo.17244360) | [Download](https://zenodo.org/records/17244360) |
| Japanese | Technical | [10.5281/zenodo.17244506](https://doi.org/10.5281/zenodo.17244506) | [Download](https://zenodo.org/records/17244506) |
| English | Technical | [10.5281/zenodo.17244558](https://doi.org/10.5281/zenodo.17244558) | [Download](https://zenodo.org/records/17244558) |

---

## Overview

The Planck-Continuous Cosmos Hypothesis proposes three broad concepts:

1. Discrete spacetime structure
   - The universe is modeled as Planck-scale cells.
   - Spacetime continuity is interpreted as an emergent network state.

2. Planck-Occupancy Saturation Principle (POSP)
   - Relativistic limits are explored through cell occupancy and saturation.
   - The speed of light is interpreted as a structural propagation limit.

3. Da-P Particles / DICP
   - Da-P particles are proposed as neutral information-cohesion agents.
   - They mediate cell-to-cell or frame-to-frame information binding.
   - Their role is theoretical and has not been experimentally confirmed.

---

## Current Numerical Status

The corrected 2025 reverification dataset reports candidate susceptibility finite-size scaling for the corrected 3D asymmetric model:

```text
chi_max ~ L^(gamma/nu)
gamma/nu ~= 2.965
R^2 ~= 0.999997
```

Available corrected system sizes:

| L | Runs | Steps | Peak p* | chi_max |
|---|------|-------|---------|---------|
| 80 | 500 | 20000 | 0.031225 | 9908.2 |
| 96 | 500 | 20000 | 0.029465 | 16975.7 |
| 128 | 500 | 20000 | 0.026650 | 39906.5 |

Limitations:

- Only three high-statistics system sizes are currently available.
- Estimates of `p_c(infinity)` and `nu` remain unstable.
- Additional sizes, independent implementation checks, and bootstrap or jackknife uncertainty analysis are needed.

---

## Cosmological Constant Residual Hypothesis

The Da-P Cosmological Constant Residual Hypothesis proposes that the cosmological constant `Lambda` may be interpreted as a global residual from imperfect synchronization of a Da-P information-cohesion network.

Candidate reformulation:

```text
Lambda = global residual of spacetime information-cohesion synchronization
```

Candidate scaling relation:

```text
Lambda_DaP * ell_P^2 ~ <(delta C / C)^2>_global ~ (ell_P / L_U)^2
```

This is a hypothesis and conceptual reformulation. It does not claim a completed derivation of the observed cosmological constant.

See:

- [docs/DaP_Cosmological_Constant_Residual_Hypothesis.md](docs/DaP_Cosmological_Constant_Residual_Hypothesis.md)
- Zenodo DOI: https://doi.org/10.5281/zenodo.20510743

---

## Data Repository

### Zenodo Records

| Record | Description | DOI |
|--------|-------------|-----|
| v1 | Initial percolation analysis | https://doi.org/10.5281/zenodo.15760964 |
| v2 | Critical exponent measurements | https://doi.org/10.5281/zenodo.16020104 |
| v3 | Finite-size scaling | https://doi.org/10.5281/zenodo.16302341 |
| v4 | Later analysis | https://doi.org/10.5281/zenodo.16522221 |
| v5 | Invalidation of previous 3D numerical claims | https://doi.org/10.5281/zenodo.16780090 |
| 2025 reverification | Corrected post-invalidation dataset | https://doi.org/10.5281/zenodo.20510158 |
| hypothesis-v1 | Cosmological constant residual hypothesis | https://doi.org/10.5281/zenodo.20510743 |

---

## Installation

```bash
git clone https://github.com/Da-P-AIP/Da-P_Particle.git
cd Da-P_Particle
pip install -r requirements.txt
```

If example scripts are available in your local checkout, run the relevant script from the `examples/` or analysis directory. The repository contents are under active revision.

---

## Documentation

For background documents, see the Zenodo records listed above.

For current update notes, see:

- [docs/DaP_2025_Reverification_Update.md](docs/DaP_2025_Reverification_Update.md)
- [docs/DaP_Cosmological_Constant_Residual_Hypothesis.md](docs/DaP_Cosmological_Constant_Residual_Hypothesis.md)

---

## Research Status

Version status: active working hypothesis under revision.

The Da-P / DICP framework remains speculative. Numerical results and theoretical interpretations should be treated as provisional unless independently reproduced and validated.

Recommended next steps:

1. Reproduce the corrected 2025 numerical results independently.
2. Add more system sizes for finite-size scaling analysis.
3. Separate raw, survival-conditioned, and corrected observables.
4. Test whether global residuals in Da-P-like networks scale as `L^-2`.
5. Compare cosmological-residual predictions with observational constraints.

---

## Contributing

This is an open research project. Contributions are welcome through issues, discussions, reproducibility checks, and pull requests.

Suggested contribution areas:

- Independent code review and simulation reproduction.
- Additional finite-size scaling analysis.
- Documentation cleanup.
- Mathematical formalization of the Da-P information-cohesion framework.
- Critical review of the cosmological constant residual hypothesis.

---

## Contact

Author: Tadashi Mazusaki  
Repository: https://github.com/Da-P-AIP/Da-P_Particle

---

## License

Code in this repository is licensed under the MIT License unless otherwise noted.

Documents are published under Creative Commons Attribution 4.0 International (CC BY 4.0) unless otherwise noted.

---

## Citation

For the corrected 2025 dataset:

```bibtex
@dataset{mazusaki2026reverification,
  title = {Corrected 2025 Reverification Results for the Da-P/DICP 3D Asymmetric Model: Candidate Anomalous Finite-Size Scaling},
  author = {Mazusaki, Tadashi},
  year = {2026},
  publisher = {Zenodo},
  doi = {10.5281/zenodo.20510158},
  url = {https://doi.org/10.5281/zenodo.20510158}
}
```

For the cosmological constant residual hypothesis:

```bibtex
@misc{mazusaki2026cosmological_residual,
  title = {The Da-P Cosmological Constant Residual Hypothesis: A Candidate Information-Cohesion Interpretation of Lambda},
  author = {Mazusaki, Tadashi},
  year = {2026},
  publisher = {Zenodo},
  doi = {10.5281/zenodo.20510743},
  url = {https://doi.org/10.5281/zenodo.20510743}
}
```

---

## Acknowledgments

This research was conducted with AI assistance for document preparation, numerical-analysis support, and research-organization workflows.

Last updated: 2026-06-02
