# Welcome to my project portfolio! 

This repository contains a selection of projects I have worked on during my studies and internships.  
Each project entry includes:
- **Synopsis**: a short overview of the work  
- **Key Results**: main findings and contributions  
- **Files**: direct links to papers, posters, or reports (when available)  

## Structure-Preserving Neural Operators, Conservation Laws, and Symplectic Flows

**Type:** Master’s Dissertation (University of Oxford)  
**Grade:** 85 / 100  
**Status:** Paper in preparation for journal submission  
**Files:** not publicly shared

### Synopsis
This dissertation develops two novel architectures for **structure-preserving operator learning**: the Quadratic First Integral Preserving DeepONet (QFIP-DeepONet) and the Symplectic Flow Network (SFN). Both models embed conservation laws directly into their architectures, aiming to improve the long-term stability of neural operator predictions on ODEs and PDEs while respecting physical structure.

### Key Results
- **QFIP-DeepONet** effectively eliminates first integral drift in ODEs and reduces generalization error, though with modest gains in pointwise accuracy.  
- **Symplectic Flow Network (SFN)** analytically preserves symplectic structure and **substantially lowers error and improved long-term stability** for ODE prediction.
- In PDE experiments (non-linear Schrödinger equation), structure-preserving models demonstrated **enhanced conservation of invariants and stability**, though not always leading to lower quantitative error.  

*Note: The full dissertation is not shared publicly as it's being prepared for publication. Please contact me if you'd like to discuss this work.*

## PINN Training via Neural Tangent Kernel: Insights and Limitations

**Type:** Course Project (Theories of Deep Learning, University of Oxford)  
**Grade:** 80 / 100  
**Date:** January 2025  
**File:** [Full Paper](NeuralTangentKernel.pdf)

### Synopsis
This project investigates the training dynamics of **physics-informed neural networks (PINNs)** using **Neural Tangent Kernel (NTK) theory**. We compared NTK-based methods with second-order optimization techniques to better understand and address the failure modes of PINN training, especially in nonlinear PDEs.


### Key Results
- Validated that NTK theory provides a theoretical explanation for failures in PINN training and motivates preconditioning techniques.  
- Showed empirically that **NTK-based models can outperform Adam and Adam+L-BFGS**, even in nonlinear PDEs (contrary to prior claims).  
- Demonstrated that **preconditioned PINNs (PCPINNs)** significantly reduce error — by **an order of magnitude** on challenging nonlinear PDEs (Heat2d-LT).  
- Found that second-order methods (e.g. Gradient-Damped Newton Descent, GDND) remain promising, achieving lowest error across multiple PDEs.

## Full Equivariant Feature Extraction for Multivectors in Clifford Group Equivariant Neural Networks

**Type:** Course Project (Geometric Deep Learning, University of Oxford)  
**Grade:** 74 / 100  
**Date:** April 2025  
**File:** [Full Paper](FEFE-CGENN.pdf)

### Synopsis
This work introduces **Full Equivariant Feature Extraction (FEFE)**, a unified framework for multivector feature extraction in Clifford Group Equivariant Neural Networks (CGENNs). Unlike previous ad-hoc methods, FEFE provides a principled, learnable approach that generalizes across tasks and improves consistency in benchmarking.

### Key Results
- Demonstrated consistent improvements across three benchmark tasks (scalar and vector prediction).  
- Reduced mean squared error (MSE) by **33–38% in low-data regimes** and by **~33% in high-data regimes** compared to original CGENN models.  
- Showed more stable learning with reduced variance across training runs.  
- Notably achieved a **4.5% reduction in error on the n-body prediction task**, indicating scalability to complex physical systems.  

## Synthetic Data Generation for Anomaly Detection in Water Pipe Networks

**Type:** Research Internship (Digital Futures Program, KTH Royal Institute of Technology)  
**Date**: August 2025  
**File:** [Poster](SyntheticDataGeneration.pdf)  
**Code:** [GitHub Repo](https://github.com/johanslettengren/synthetic-anomaly-generation)

### Synopsis
This project explored the use of **physics-informed neural networks (PINNs)** to accelerate simulations of water pipe networks, which are typically performed using EPANET. The key focus was on generating large volumes of **synthetic data for leak scenarios** via amortized prediction, enabling scalable anomaly detection in settings where real leaks are rare. By embedding governing hydraulic equations into the learning process, the PINN model generalized across multiple leak scenarios simultaneously, achieving accurate flow predictions while substantially reducing computational costs.

### Key Results
- PINN-based amortized data generation produced accurate predictions (NRMSD ≤ 10%) across leak scenarios.  
- Showed strong scalability compared to traditional one-simulation-per-scenario methods.  
- Demonstrated reduced runtime for large parameter sweeps (e.g., PINN outperformed simulator at higher grid resolutions and number of demand junctions).

## Evaluating Brain-Inspired Models for Time Series Forecasting

**Type:** Bachelor Thesis (KTH Royal Institute of Technology)  
**Date:** June 2023  
**File:** [Full Thesis](BachelorThesis.pdf)  

### Synopsis
This thesis investigates the potential of **brain-inspired machine learning models** for time series forecasting, with a focus on their ability to capture and exploit **dynamical memory**. Three approaches were implemented: a vanilla recurrent neural network (VRNN), a reservoir computing (RC) model, and a time-lagged reservoir computing (TLRC) model. For benchmarking, results were compared against the traditional statistical method ARIMA. The models were evaluated across both benchmark datasets (Mackey–Glass and Lorenz systems) and experimental data, including financial, environmental, and EEG recordings.  

### Key Results
- **Reservoir computing models** consistently outperformed VRNN in terms of stability and accuracy, particularly in chaotic benchmark datasets.  
- **TLRC** showed the strongest performance in two out of three univariate datasets, demonstrating that explicit use of historical information can boost predictive accuracy.  
- Memory analysis showed that reservoir models capture historical dependencies.  
