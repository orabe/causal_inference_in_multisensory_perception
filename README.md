# Causal Inference in Multisensory Perception

Implementation and analysis of a Bayesian causal inference model for multisensory perception based on:

Koerding, K. P., Beierholm, U., Ma, W. J., Quartz, S., Tenenbaum, J. B., & Shams, L. (2007). *Causal inference in multisensory perception*. PLoS ONE, 2(9), e943.  [oai_citation:0‡mhbf_project_multi_sensory_integrations_Ammar-Mohammd.pdf](sediment://file_00000000bfb871f4bd1aab59097bb26f)

## Overview

This project investigates how an optimal Bayesian observer integrates visual and auditory sensory information while inferring whether both signals originate from a common source.

The implemented model:

- Simulates multisensory perception experiments
- Estimates stimulus locations from noisy sensory observations
- Infers the probability of a common cause
- Generates synthetic experimental data
- Fits model parameters using:
  - Brute-force parameter search
  - Markov Chain Monte Carlo (MCMC)

## Repository Structure

```text
.
├── project_summary.pdf          # Project report
├── multisensory_causal_inference.ipynb
└── README.md
```

## Model Parameters

The Bayesian causal inference model is characterized by:

| Parameter | Description |
|------------|------------|
| p_common | Prior probability of a common cause |
| σ_v | Visual uncertainty |
| σ_a | Auditory uncertainty |
| μ_p | Spatial prior mean |
| σ_p | Spatial prior variance |

## Main Experiments

- Analysis of posterior common-cause probability
- Effect of sensory uncertainty on stimulus estimation
- Synthetic data generation
- Parameter recovery via likelihood maximization
- Comparison of brute-force search and MCMC sampling
- Parameter estimation on heterogeneous datasets

## Results

Key findings include:

- Higher prior belief in a common cause increases sensory integration.
- Increased sensory uncertainty shifts estimates toward the more reliable modality.
- MCMC provides more accurate parameter recovery than brute-force search.
- Parameter dependencies make marginal likelihood interpretation challenging.

## Requirements

Typical dependencies:

```bash
numpy
scipy
matplotlib
pandas
emcee
jupyter
```

## Running

Open the notebook:

```bash
jupyter notebook multisensory_causal_inference.ipynb
```

and execute all cells to reproduce simulations, figures, and model fitting results.

## Author

[Mohammad Orabe](https://github.com/orabe-mhd)

[Ammar Ibrahim](https://github.com/Ammar-Elsaeed)

Models of Higher Brain Functions (MHBF)
TU Berlin
