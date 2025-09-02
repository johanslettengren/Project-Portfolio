## Structure-Preserving Neural Operators, Conservation Laws, and Symplectic Flows

**Type:** Master’s Dissertation (University of Oxford)  
**Status:** Manuscript in preparation for journal submission (not publicly shared)  

### Synopsis
This dissertation explores the emerging field of **structure-preserving operator learning**, at the intersection of geometric numerical integration and scientific machine learning. The work introduces two novel architectures — the **Quadratic First Integral Preserving DeepONet (QFIP-DeepONet)** and the **Symplectic Flow Network (SFN)** — designed to respect conservation laws and symplectic structure in dynamical systems. These models aim to improve long-term stability of neural operator predictions without sacrificing accuracy.

### Key Results
- **QFIP-DeepONet** effectively eliminates first integral drift in ODEs and reduces generalization error, though with modest gains in pointwise accuracy.  
- **Symplectic Flow Network (SFN)** achieves **substantially lower error and improved long-term stability**, validating symplectic structure as a powerful inductive bias.  
- In PDE experiments (non-linear Schrödinger equation), structure-preserving models demonstrated **enhanced conservation of invariants and stability**, though not always leading to lower quantitative error.  

### Outlook
By embedding geometric structure directly into neural operator architectures, this work contributes to the development of reliable, physically-consistent scientific machine learning models. Extensions include broader applications to Hamiltonian PDEs, more complex conservation laws, and hybrid operator-integrator approaches.

*Note: The full dissertation is not shared publicly as it is being prepared for publication. Please contact me if you are interested in discussing this work.*

## PINN Training via Neural Tangent Kernel: Insights and Limitations

**Type:** Course Project (Theories of Deep Learning, University of Oxford)  
**Grade:** 80 / 100  
**Date:** January 2025  
**File:** [Full Paper (PDF)](https://github.com/johanslettengren/Research-Projects/blob/main/NeuralTangentKernel.pdf)

### Abstract
This paper investigates the training dynamics of PINNs to address challenges in optimizing their loss functions. We review results from NTK theory, which explain common failures in PINN training and motivate preconditioning techniques to improve the loss landscape. While NTK theory offers valuable insights, certain results break down in the case of nonlinear PDEs. To address this, we explore second-order methods as a potential solution. Through numerical experiments, we validate NTK-based models and demonstrate their effectiveness in both linear and nonlinear regimes. Additional experiments show that preconditioning techniques and second-order methods outperform traditional optimizers, highlighting their potential for robust PINN training.

### Key Results
- Validated that NTK theory provides a theoretical explanation for failures in PINN training and motivates preconditioning techniques.  
- Showed empirically that **NTK-based models can outperform Adam and Adam+L-BFGS**, even in nonlinear PDEs (contrary to prior claims).  
- Demonstrated that **preconditioned PINNs (PCPINNs)** significantly reduce error — by **an order of magnitude** on challenging nonlinear PDEs (Heat2d-LT).  
- Found that second-order methods (e.g. Gradient-Damped Newton Descent, GDND) remain promising, achieving lowest error across multiple PDEs.

## Full Equivariant Feature Extraction for Multivectors in Clifford Group Equivariant Neural Networks

**Type:** Course Project (Geometric Deep Learning, University of Oxford)  
**Grade:** 74 / 100  
**Date:** April 2025  
**File:** [Full Paper (PDF)](https://github.com/johanslettengren/Research-Projects/blob/main/FEFE-CGENN.pdf)

### Abstract
We propose a general, learnable framework for multivector feature extraction in Clifford Group Equivariant Neural Networks (CGENNs), which addresses a key limitation in existing models. Our method—termed Full Equivariant Feature Ex- traction for Multivectors (FEFE)—leverages grade-wise projections and geomet- ric products to unify and extend previous ad-hoc approaches. We demonstrate improved performance across three benchmark tasks, including scalar and vector predictions.

### Key Results
- Demonstrated consistent improvements across three benchmark tasks (scalar and vector prediction).  
- Reduced mean squared error (MSE) by **33–38% in low-data regimes** and by **~33% in high-data regimes** compared to original CGENN models.  
- Showed more stable learning with reduced variance across training runs.  
- Notably achieved a **4.5% reduction in error on the n-body prediction task**, indicating scalability to complex physical systems.  

## Synthetic Data Generation for Anomaly Detection in Water Pipe Networks

**Type:** Research Internship (Digital Futures Program, KTH Royal Institute of Technology)  
**Date**: August 2025

**Presented as:** Poster at Digital Futures Research Internship Symposium

**File:** [Poster (PDF)](SyntheticDataGeneration.pdf)

### Synopsis
This project explored the use of **physics-informed neural networks (PINNs)** to accelerate simulations of water pipe networks, which are typically performed using EPANET. The key focus was on generating large volumes of **synthetic data for leak scenarios** via amortized prediction, enabling scalable anomaly detection in settings where real leaks are rare. By embedding governing hydraulic equations into the learning process, the PINN model generalized across multiple leak scenarios simultaneously, achieving accurate flow predictions while substantially reducing computational costs.

### Key Results
- PINN-based amortized data generation produced accurate predictions (NRMSD ≤ 10%) across leak scenarios.  
- Showed strong scalability compared to traditional one-simulation-per-scenario methods.  
- Demonstrated reduced runtime for large parameter sweeps (e.g., PINN outperformed simulator at higher grid resolutions and number of demand junctions).  
