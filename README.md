## PINN Training via Neural Tangent Kernel: Insights and Limitations

**Type:** Course project (Theories of Deep Learning, University of Oxford)  
**Grade:** 8.0 / 10.0  
**Date:** 2024  
**File:** [[Full Paper (PDF)]((https://github.com/johanslettengren/Research-Projects/blob/main/NeuralTangentKernel.pdf))]

### Abstract
This paper investigates the training dynamics of PINNs to address challenges in optimizing their loss functions. We review results from NTK theory, which explain common failures in PINN training and motivate preconditioning techniques to improve the loss landscape. While NTK theory offers valuable insights, certain results break down in the case of nonlinear PDEs. To address this, we explore second-order methods as a potential solution. Through numerical experiments, we validate NTK-based models and demonstrate their effectiveness in both linear and nonlinear regimes. Additional experiments show that preconditioning techniques and second-order methods outperform traditional optimizers, highlighting their potential for robust PINN training.
