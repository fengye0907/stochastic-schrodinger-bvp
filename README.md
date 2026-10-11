# Stochastic Schrödinger equation with boundary condition in time — numerical experiments

This repository contains the Jupyter notebook accompanying the paper

> R. Pettersson, A. Sirma, Z. Feng.
> *Stochastic Schrödinger equation with boundary condition in time and additive noise: Truncation error and simulation algorithms.*

The paper studies a linear stochastic Schrödinger equation driven by a trace-class $Q$-Wiener process, subject to a two-point temporal boundary condition $re^{i\theta}u(0)=u(T)$. The notebook implements the simulation algorithms from the paper and reproduces its numerical experiments:

- the **truncated exact solution** (spectral truncation to $J$ modes) and its truncation error;
- the **exponential-integrator-type time discretization** and its time-discretization error;
- empirical convergence rates compared with the theoretical ones.

## Contents

| File | Description |
|------|-------------|
| `truncation_error_simulation.ipynb` | Implementation of the algorithms and all numerical experiments (with saved outputs/figures) |
| `requirements.txt` | Python dependencies |

## Usage

Requires Python ≥ 3.9.

```bash
pip install -r requirements.txt
jupyter notebook truncation_error_simulation.ipynb
```

All random number generators are seeded, so the results are reproducible.

## Citation

If you use this code, please cite the paper above (see also `CITATION.cff`).

## Contact

Zijie Feng — fengye0907@outlook.com

## License

Released under the MIT License — see `LICENSE`.
