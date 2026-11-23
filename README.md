# Continual Learning in the Time-Series Domain

**Research on continual learning, forecasting, and adaptive representation learning for evolving time-series data.**

This repository is part of the [Collab-Multimodal-Lifelong-Learning](https://github.com/Collab-Multimodal-Lifelong-Learning) project, **Developing a Sustainable Collaborative Multi-modal Lifelong Learning Framework**. It brings together research on representing structured temporal patterns, adapting models to changing signal characteristics, and detecting critical changes in time-series data.

Browse the [12 research projects](#code-and-resources) for source code and documentation.

## Research Overview

Time-series data from real-world environments are rarely stationary. Their trends, periodicities, noise characteristics, sampling rates, and operating conditions may change over time. A sustainable learning system should recognize these structures, adapt its predictions to new conditions, and detect meaningful changes while preserving useful knowledge from earlier observations.

Within the project's **PDM (Pre-trained, Data, Memory)** perspective, this repository focuses on the **time-series data domain**, complementing the project's vision, language, and general continual-learning research. The methods covered here contribute to the foundations of time-series continual learning; individual forecasting and anomaly-detection studies should not automatically be interpreted as evaluations of a complete end-to-end continual-learning framework.

The principal research directions are:

1. **Structured Time-Series Representation Learning:** Decomposing temporal observations into interpretable components and modeling latent sources of change and uncertainty.
2. **Structure-Aligned and Separable Learning:** Learning heterogeneous temporal patterns through appropriately separated training objectives and gradient pathways.
3. **Function-to-Function Time-Series Modeling:** Learning flexible time-series representations and context-dependent prediction functions that can generalize across sampling conditions.
4. **Critical-Transition Anomaly Detection and Continual Adaptation:** Identifying important transitions from temporal signals and extending time-series models toward changing-task environments.

## Research Directions

### 1. Structured Time-Series Representation Learning

**Research focus:** Discovering and representing the underlying components of evolving time-series signals.

- Characterize temporal variation through factors such as **trend**, **periodic structure**, **residual fluctuations**, and **uncertainty**.
- Explore representations that distinguish **system drift** from variation associated with human or environmental factors.
- Investigate uncertainty-aware temporal modeling, including structured stochastic priors for latent effects.
- Extract dominant signal components iteratively so that remaining residuals can be modeled separately rather than forcing a single predictor to explain all temporal structure at once.

**Representative research:** *SHIFTS* and the iterative decomposition component of *SALT*.

**Research team:** Prof. Noseong Park, KAIST.

### 2. Structure-Aligned and Separable Learning

**Research focus:** Reducing interference between temporal components during forecasting-model training.

- Study how jointly optimizing signals with different frequency characteristics can introduce **gradient interference** and **spectral bias**.
- Decompose an observed series into dominant components and residual structure through **Iterative Dominant Extraction (IDE)**.
- Train component-specific predictors and losses separately to improve the learning of both dominant and less prominent patterns.
- Investigate whether structure-aware training can be applied across different forecasting backbones and distributional conditions.

**Representative research:** *SALT — Structure-Aligned Learning for Time-Series Forecasting*.

**Research team:** Prof. Noseong Park, KAIST.

### 3. Function-to-Function Time-Series Modeling

**Research focus:** Modeling a time series as a function and learning mappings between observed and predicted temporal functions.

- Investigate **operator-learning** approaches that map an input time-series function to a future function rather than treating every observation as a fixed-length vector.
- Explore multiple functional bases, including **Fourier**, **radial basis functions (RBF)**, **polynomial**, and higher-frequency components.
- Study **hypernetwork / hyper-head** mechanisms that generate context-dependent parameters for different functional representations.
- Improve generalization across temporal resolutions and changes in sampling rate, while providing a foundation for future task-conditioned continual updates.

**Representative research:** *TimeOperator — A Function-to-Function Approach to Time Series Modeling*.

**Research team:** Prof. Noseong Park, KAIST.

### 4. Critical-Transition Anomaly Detection and Continual Adaptation

**Research focus:** Detecting meaningful temporal changes and supporting adaptation when operating conditions evolve.

- Detect **point-wise anomalies** by estimating how closely a system approaches a critical state transition.
- Combine sensitivity and uncertainty signals from a forecasting model and accumulate them through **fold-bifurcation-inspired ordinary differential equation (ODE)** dynamics.
- Distinguish transient prediction-error spikes from changes that emerge through accumulated stress.
- Investigate task conditioning, distribution changes, and evaluation protocols for extending time-series models toward continual-learning scenarios.

**Representative research:** *FOLD — Point-wise Anomaly Detection via Fold-bifurcation ODE*.

**Research team:** Prof. Noseong Park, KAIST.

## Representative Research and Publications

The following works are highlighted in the project's July 15, 2026 progress evaluation.

### Published or Accepted Research

- **[TimeOperator: A Function-to-Function Approach to Time Series Modeling](https://neurips.cc/virtual/2026/poster/155398)** — *NeurIPS 2026*.
  - Studies function-to-function modeling, multiple functional bases, and context-dependent modeling of time-series signals.

- **[Point-wise Anomaly Detection via Fold-bifurcation ODE (FOLD)](https://proceedings.iclr.cc/paper_files/paper/2026/hash/19dc8bc893019f7317df1c3bb30bffe2-Abstract-Conference.html)** — *ICLR 2026*.
  - Models anomaly detection as an approach toward a critical transition, using stress signals and fold-bifurcation-inspired dynamics under a point-wise evaluation protocol.
  - [FOLD code and documentation](https://github.com/Collab-Multimodal-Lifelong-Learning/FOLD/blob/00ec9e16c32adfa236f893ad795c2c784736731e/README.md)

### Additional Project-Described Research

- **SALT: Structure-Aligned Learning for Time-Series Forecasting** — *Research manuscript described in the July 2026 project evaluation; final publication status not asserted here*.
  - Combines **Iterative Dominant Extraction** and **Separable Training** to reduce gradient interference and improve learning across temporal structures.

- **SHIFTS: Modeling Human Factors in Time Series via Structured Uncertainty** — *2026 project-described research; publication status not asserted here*.
  - Investigates separation of system drift and human-factor variation, with structured modeling of latent temporal uncertainty.

## Evaluation Highlights

The following numbers are **project-reported results** from the progress-evaluation materials dated **July 15, 2026**. They are **not independently reproduced from code in this repository**. Mean squared error (MSE) is a lower-is-better metric.

| Evaluation task | Benchmark | Metric | Project target (2026) | Reported result (2026) |
| --- | --- | --- | ---: | ---: |
| Time-series forecasting | ETTh1 | MSE ↓ | 0.478 | **0.329** |
| Multivariate time-series forecasting | PeMS03 | MSE ↓ | 0.125 | **0.110** |

**Evaluation context:** The project reports forecasting results on **ETTh1** and **PeMS03** in its overall performance-indicator table. Its time-series appendix additionally discusses method-specific results (including TimeOperator on ETTh1 and Weather); these figures are not necessarily measured under identical model and evaluation configurations and should not be conflated with the summary metrics above.

### Evaluation Topics

| Topic | Example evaluation focus |
| --- | --- |
| Time-series forecasting | Forecasting error under evolving temporal conditions |
| Multivariate forecasting | Accuracy across correlated temporal variables |
| Temporal-pattern decomposition | Component separation and robustness to heterogeneous patterns |
| Point-wise anomaly detection | Sensitivity to critical transitions under strict point-wise evaluation |
| Continual time-series adaptation | Forgetting, forward/backward transfer, and task-conditioned adaptation |

## Code and Resources

Each project is a Git submodule pinned to a commit in its organization fork. The table links to that revision's README and lists both the fork and its upstream repository.

Clone this repository and its project folders with:

```bash
git clone --recurse-submodules --shallow-submodules https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Time-Series-Domain.git
```

In an existing checkout, run `git submodule update --init --recursive --depth 1`.

| Project README | Research focus | Repositories |
| --- | --- | --- |
| [GT-GAN](https://github.com/Collab-Multimodal-Lifelong-Learning/GT-GAN/blob/360c79edb08c09c2b018483c7dd7ddd18533a8cd/README.md) | Generative adversarial networks for time-series synthesis. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/GT-GAN) · [Upstream](https://github.com/Jinsung-Jeon/GT-GAN) |
| [LEAP](https://github.com/Collab-Multimodal-Lifelong-Learning/LEAP/blob/a5749ad782b0f780a1f78a7de6b8b4b5d18f4202/README.md) | Learnable paths for neural controlled differential equations. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/LEAP) · [Upstream](https://github.com/minju-hi/LEAP) |
| [Hawkes-Process-Based-on-Controlled-Differential-Equations](https://github.com/Collab-Multimodal-Lifelong-Learning/Hawkes-Process-Based-on-Controlled-Differential-Equations/blob/ee58a4622b9bb76339c07c94ee0fa758416b1dbb/README.md) | Continuous-time event modeling with Hawkes processes and controlled differential equations. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/Hawkes-Process-Based-on-Controlled-Differential-Equations) · [Upstream](https://github.com/kookseungji/Hawkes-Process-Based-on-Controlled-Differential-Equations) |
| [pad](https://github.com/Collab-Multimodal-Lifelong-Learning/pad/blob/ca0e9b0402f13b4042aac3f9d89770437f7d0507/README.md) | Detection of anomalies and their precursors in irregular time series. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/pad) · [Upstream](https://github.com/sheoyon-jhin/pad) |
| [NADE](https://github.com/Collab-Multimodal-Lifelong-Learning/NADE/blob/c4850e61483979c460a591651bd9bd415e122ab1/readme.md) | Climate modeling with a neural advection–diffusion equation. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/NADE) · [Upstream](https://github.com/hwangyong753/NADE) |
| [BSARec](https://github.com/Collab-Multimodal-Lifelong-Learning/BSARec/blob/c80bdc0f1a889b78fe9a27e2058389cc84caea84/README.md) | Sequential recommendation with an inductive bias that complements self-attention. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/BSARec) · [Upstream](https://github.com/yehjin-shin/BSARec) |
| [CONTIME](https://github.com/Collab-Multimodal-Lifelong-Learning/CONTIME/blob/5ac3f44f136447315aca506b6540bc31c9d31cb3/README.md) | Continuous-time forecasting with derivative regularization to reduce prediction delay. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/CONTIME) · [Upstream](https://github.com/sheoyon-jhin/CONTIME) |
| [NCDENow_CIKM2024](https://github.com/Collab-Multimodal-Lifelong-Learning/NCDENow_CIKM2024/blob/7e6123313be0047fe27b1251761bae278b1797df/README.md) | GDP nowcasting with dynamic factor models and neural controlled differential equations. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/NCDENow_CIKM2024) · [Upstream](https://github.com/sklim84/NCDENow_CIKM2024) |
| [ANCDE](https://github.com/Collab-Multimodal-Lifelong-Learning/ANCDE/blob/cce222f4602eae3dd2e0fbf069e20c6798dbd48e/README.md) | Attentive neural controlled differential equations for time-series classification and forecasting. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/ANCDE) · [Upstream](https://github.com/sheoyon-jhin/ANCDE) |
| [TV-Rec](https://github.com/Collab-Multimodal-Lifelong-Learning/TV-Rec/blob/0ed874e9791c58bf8ad3715208e4d4e3ece19381/README.md) | Time-varying convolutional filters for sequential recommendation. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/TV-Rec) · [Upstream](https://github.com/yehjin-shin/TV-Rec) |
| [TABLeT](https://github.com/Collab-Multimodal-Lifelong-Learning/TABLeT/blob/a36f5a2bd728d0530100b48415f0aadc976ee593/README.md) | Tokenization of fMRI volumes for long-range spatiotemporal modeling. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/TABLeT) · [Upstream](https://github.com/beotborry/TABLeT) |
| [FOLD](https://github.com/Collab-Multimodal-Lifelong-Learning/FOLD/blob/00ec9e16c32adfa236f893ad795c2c784736731e/README.md) | Point-wise anomaly detection using fold-bifurcation dynamics. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/FOLD) · [Upstream](https://github.com/sheoyon-jhin/FOLD) |

## Related Repositories

Other research areas within [Collab-Multimodal-Lifelong-Learning](https://github.com/Collab-Multimodal-Lifelong-Learning):

- [Continual-Learning-Vision-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Vision-Domain) — Continual learning in the vision domain.
- [Continual-Learning-Language-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Language-Domain) — Continual learning for language models and evolving knowledge.
- [Continual-Learning-and-Multimodal-Integration](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-and-Multimodal-Integration) — General continual-learning methods, memory, and multimodal integration.
- [PDM-Framework](https://github.com/Collab-Multimodal-Lifelong-Learning/PDM-Framework) — Project-level PDM continual-learning framework.

## Acknowledgment

This research is associated with the Korean national R&D project **“Developing a Sustainable Collaborative Multi-modal Lifelong Learning Framework” (Project No. 2022-0-00113)**, conducted within the *Human-Centered AI Core Technology Development* program, supported by the Ministry of Science and ICT (MSIT) and administered by the Institute of Information & Communications Technology Planning & Evaluation (IITP).
