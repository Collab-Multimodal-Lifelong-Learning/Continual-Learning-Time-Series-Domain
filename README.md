# Continual Learning in the Time-Series Domain

**Research on continual learning, forecasting, and adaptive representation learning for evolving time-series data.**

This repository is part of the [Collab-Multimodal-Lifelong-Learning](https://github.com/Collab-Multimodal-Lifelong-Learning) project, **Developing a Sustainable Collaborative Multi-modal Lifelong Learning Framework**. It brings together research on representing structured temporal patterns, adapting models to changing signal characteristics, and detecting critical changes in time-series data.

## Research list

### Time-series synthesis, modeling, and forecasting

- **GT-GAN: General Purpose Time Series Synthesis with Generative Adversarial Networks** (NeurIPS 2022) — Jinsung Jeon et al.
  - Synthesizes both regularly and irregularly sampled time series with a common architecture.
  - [Paper](https://arxiv.org/abs/2210.02040) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/GT-GAN/blob/fc1f20ef1dbffb8d72c84712c215440ec71ce696/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/GT-GAN) · [Upstream](https://github.com/Jinsung-Jeon/GT-GAN)

- **Attentive Neural Controlled Differential Equations for Time-Series Classification and Forecasting (ANCDE)** (ICDM 2021) — Sheo Yon Jhin et al.
  - Attentive neural controlled differential equations for time-series classification and forecasting.
  - [Paper](https://arxiv.org/abs/2109.01876) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/ANCDE/blob/c0c0e26d80ba4882d991972b81cb7d1cb4f14262/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/ANCDE) · [Upstream](https://github.com/sheoyon-jhin/ANCDE)

- **Learnable Path in Neural Controlled Differential Equations (LEAP)** (AAAI 2023) — Sheo Yon Jhin et al.
  - Learnable paths for neural controlled differential equations.
  - [Paper](https://arxiv.org/abs/2301.04333) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/LEAP/blob/bd49fe865c59ae09d71d24b0ef0fd9b7bf4b4702/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/LEAP) · [Upstream](https://github.com/minju-hi/LEAP)

- **Hawkes Process Based on Controlled Differential Equations** (IJCAI 2023) — Minju Jo, Seungji Kook, and Noseong Park
  - Continuous-time event modeling with Hawkes processes and controlled differential equations.
  - [Paper](https://www.ijcai.org/proceedings/2023/239) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/Hawkes-Process-Based-on-Controlled-Differential-Equations/blob/50c07c354a9f42a5b8a05acb201e4fc408986788/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/Hawkes-Process-Based-on-Controlled-Differential-Equations) · [Upstream](https://github.com/kookseungji/Hawkes-Process-Based-on-Controlled-Differential-Equations)

- **Climate Modeling with Neural Advection-Diffusion Equation (NADE)** (ICML 2023) — Hwangyong Choi et al.
  - Climate modeling with a neural advection–diffusion equation.
  - [Paper](https://proceedings.mlr.press/v202/choi23a.html) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/NADE/blob/3882b68a5c237f409b0a6b9d9138e859bdca3e7f/readme.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/NADE) · [Upstream](https://github.com/hwangyong753/NADE)

- **Addressing Prediction Delays in Time Series Forecasting: A Continuous GRU Approach with Derivative Regularization (CONTIME)** (KDD 2024) — Sheo Yon Jhin, Seojin Kim, and Noseong Park
  - Regularizes time derivatives in a continuous-time GRU to reduce the lag between forecasts and observations.
  - [Paper](https://arxiv.org/abs/2407.01622) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/CONTIME/blob/e48da62889131021534e5519c337b543386e086b/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/CONTIME) · [Upstream](https://github.com/sheoyon-jhin/CONTIME)

- **Bridging Dynamic Factor Models and Neural Controlled Differential Equations for Nowcasting GDP (NCDENow)** (CIKM 2024) — Seonkyu Lim et al.
  - GDP nowcasting with dynamic factor models and neural controlled differential equations.
  - [Paper](https://arxiv.org/abs/2409.08732) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/NCDENow_CIKM2024/blob/32dc54c19e3f6edc2932c1f4588ea661468ec985/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/NCDENow_CIKM2024) · [Upstream](https://github.com/sklim84/NCDENow_CIKM2024)

- **Can Natural Image Autoencoders Compactly Tokenize fMRI Volumes for Long-Range Dynamics Modeling? (TABLeT)** (CVPR 2026) — Peter Yongho Kim et al.
  - Tokenization of fMRI volumes for long-range spatiotemporal modeling.
  - [Paper](https://arxiv.org/abs/2604.03619) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/TABLeT/blob/1c614c1704a7962dbe48f302fdc87b05947a9cb2/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/TABLeT) · [Upstream](https://github.com/beotborry/TABLeT)

### Anomaly and precursor detection

- **Precursor-of-Anomaly Detection for Irregular Time Series** (KDD 2023) — Sheo Yon Jhin, Jaehoon Lee, and Noseong Park
  - Detection of anomalies and their precursors in irregular time series.
  - [Paper](https://arxiv.org/abs/2306.15489) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/pad/blob/96ba1c2ae241059af02bd9db3d8dd648c73535b3/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/pad) · [Upstream](https://github.com/sheoyon-jhin/pad)

- **Point-wise Anomaly Detection via Fold-bifurcation ODE (FOLD)** (ICLR 2026) — Sheo Yon Jhin and Noseong Park
  - Models anomaly detection as an approach toward a critical transition, using stress signals and fold-bifurcation-inspired dynamics under a point-wise evaluation protocol.
  - [Paper](https://proceedings.iclr.cc/paper_files/paper/2026/hash/19dc8bc893019f7317df1c3bb30bffe2-Abstract-Conference.html) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/FOLD/blob/522e7d0e1fbc389905601de284bf3afd748c7d6f/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/FOLD) · [Upstream](https://github.com/sheoyon-jhin/FOLD)

### Sequential recommendation

- **An Attentive Inductive Bias for Sequential Recommendation beyond the Self-Attention (BSARec)** (AAAI 2024) — Yehjin Shin et al.
  - Sequential recommendation with an inductive bias that complements self-attention.
  - [Paper](https://arxiv.org/abs/2312.10325) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/BSARec/blob/95c5a90414353cc39c639fb80787b379349d9873/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/BSARec) · [Upstream](https://github.com/yehjin-shin/BSARec)

- **TV-Rec: Time-Variant Convolutional Filter for Sequential Recommendation** (NeurIPS 2025) — Yehjin Shin et al.
  - Time-varying convolutional filters for sequential recommendation.
  - [Paper](https://arxiv.org/abs/2510.25259) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/TV-Rec/blob/b74860476afbd6c8e1f245c3da41c764d043dd7a/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/TV-Rec) · [Upstream](https://github.com/yehjin-shin/TV-Rec)

### Additional project research

The following works are highlighted in the project's July 15, 2026 progress evaluation.

#### Published or Accepted Research

- **[TimeOperator: A Function-to-Function Approach to Time Series Modeling](https://neurips.cc/virtual/2026/poster/155398)** — *NeurIPS 2026*.
  - Studies function-to-function modeling, multiple functional bases, and context-dependent modeling of time-series signals.

#### Additional Project-Described Research

- **SALT: Structure-Aligned Learning for Time-Series Forecasting** — *Research manuscript described in the July 2026 project evaluation; final publication status not asserted here*.
  - Combines **Iterative Dominant Extraction** and **Separable Training** to reduce gradient interference and improve learning across temporal structures.

- **SHIFTS: Modeling Human Factors in Time Series via Structured Uncertainty** — *2026 project-described research; publication status not asserted here*.
  - Investigates separation of system drift and human-factor variation, with structured modeling of latent temporal uncertainty.

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

Each Project code link opens the README at the pinned commit in the organization fork. The corresponding submodule uses the same revision. Open the upstream repository for the original source.

Clone this repository and its project folders with:

```bash
git clone --recurse-submodules --shallow-submodules https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Time-Series-Domain.git
```

In an existing checkout, run `git submodule update --init --recursive --depth 1`.

## Related Repositories

Other research areas within [Collab-Multimodal-Lifelong-Learning](https://github.com/Collab-Multimodal-Lifelong-Learning):

- [Continual-Learning-Vision-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Vision-Domain) — Continual learning in the vision domain.
- [Continual-Learning-Language-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Language-Domain) — Continual learning for language models and evolving knowledge.
- [Continual-Learning-and-Multimodal-Integration](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-and-Multimodal-Integration) — General continual-learning methods, memory, and multimodal integration.
- [PDM-Framework](https://github.com/Collab-Multimodal-Lifelong-Learning/PDM-Framework) — Project-level PDM continual-learning framework.

## Acknowledgment

This research is associated with the Korean national R&D project **“Developing a Sustainable Collaborative Multi-modal Lifelong Learning Framework” (Project No. 2022-0-00113)**, conducted within the *Human-Centered AI Core Technology Development* program, supported by the Ministry of Science and ICT (MSIT) and administered by the Institute of Information & Communications Technology Planning & Evaluation (IITP).
