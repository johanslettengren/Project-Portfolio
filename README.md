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
**Presented as:** Poster at Digital Futures Research Internship Symposium, 2025
**File:** [Poster (PDF)](SyntheticDataGeneration.pdf)

### Synopsis
This project explored the use of **physics-informed neural networks (PINNs)** to accelerate simulations of water pipe networks, which are typically performed using EPANET. The key focus was on generating large volumes of **synthetic data for leak scenarios** via amortized prediction, enabling scalable anomaly detection in settings where real leaks are rare. By embedding governing hydraulic equations into the learning process, the PINN model generalized across multiple leak scenarios simultaneously, achieving accurate flow predictions while substantially reducing computational costs.

### Key Results
- PINN-based amortized data generation produced accurate predictions (NRMSD ≤ 10%) across leak scenarios.  
- Showed strong scalability compared to traditional one-simulation-per-scenario methods.  
- Demonstrated reduced runtime for large parameter sweeps (e.g., PINN outperformed simulator at higher grid resolutions and number of demand junctions).  
