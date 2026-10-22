# Sparse Bayesian DOA Estimation with Baseline Correction: A Sparse Bayesian Learning Method[with MATLAB Code]

Analysis of Spectral Techniques in Analytical Chemistry: In practical applications, spectral techniques often suffer from baseline effects. Without baseline correction, the accuracy of qualitative/quantitative analysis results can be significantly compromised. Recently, sparse representation has been applied to baseline correction, offering state-of-the-art performance. However, it experiences a potential performance drop when implementing an L1 norm approximation. To significantly enhance baseline correction performance, a joint pure spectral fitting and baseline correction framework for Sparse Bayesian Learning (SBL) is proposed in this work. Due to the SBL framework's high flexibility in addressing the minimum L0 norm problem rather than an L1 norm approximation, it is possible to achieve higher baseline correction precision. Moreover, the proposed method possesses inherent learning capabilities, thus eliminating the need for additional regularization terms. Note that if the grid points used in the dictionary matrix are not sufficiently dense, the performance of sparse representation will decrease. Therefore, we further consider grid points as adjustable parameters, followed by grid refinement techniques to handle off-grid gaps. Simulations and real datasets show that the proposed SBL-based method offers substantial performance improvements over existing schemes in baseline correction.
To overcome the aforementioned shortcomings of SSFBCSP, in this paper, we propose a framework for Sparse Bayesian Learning (SBL) that integrates pure spectral fitting with baseline correction. It is worth noting that when the signal of interest is specified as a Laplace prior, methods based on l1 norm actually equate to the maximum a posteriori (MAP) estimation [25]. Although the SBL framework also attempts to recover sparse signals of interest using an MAP estimator, it provides a flexible way to select priors for the signals of interest. Both existing theoretical and empirical results indicate that SBL methods with better prior information can achieve enhanced performance over L1 norm-based methods [25, 26]. Therefore, it is expected that the proposed SBL-based method will outperform SSFBCSP. Another advantage of the proposed method is that the SBL framework inherently possesses learning capabilities, thus excluding the need for regularization terms. Additionally, to handle off-grid gaps in dictionary matrices, we further consider grid points as adjustable parameters, followed by grid refinement techniques [20] to enhance signal recovery. Simulations and experimental results on both simulated and real datasets show that the method is superior to existing methods, especially under low Signal-to-Noise Ratio (SNR) conditions.
As far as we know, there are no SBL-based methods that jointly estimate sparse signals and correct baselines in the literature. Note that in [27], a mixed Bayesian model is applied to characterize the baseline and peak, and then an expectation maximization (EM) algorithm is proposed to fit the baseline with P-spline. However, the convergence and optimality of the EM algorithm cannot be guaranteed theoretically, which may reduce performance. As shown later, our SBL-based solution is completely different from the above mixed Bayesian model approach. The rest of this paper is organized as follows. Section 2 presents a sparse Bayesian formulation of baseline correction and corresponding Bayesian inference, along with a dictionary handling off-grid gaps through grid refinement technology. Section 3 reports simulation and real dataset results. Finally, conclusions are presented in Section 4.
The SBL-based baseline correction (SBL-BC) algorithm is outlined in Section 1.
Simulation and Experiment
More radar and communication MATLAB codes
clear\nclose all\n\nload noise.mat\nload chromatogram.mat;\ny=X(:,5)+ noise;\n\ntic;\n[w,A,b]=SBL_BC(y);\ntoc\ns=A*w;\n\nfigure(1);plot(y,'b');hold on; plot(s ,'r'); plot(b,'g'); hold off;\nlegend('original spectrum','estimated spectrum','estimated baseline')\ntitle('SBL-BC')\n  

## Images

![Sparse Bayesian DOA Estimation with Baseline Correction - Sparse Bayesian Learning Method with Baseline Correction [with MATLAB Code]](01.jpg)
![Sparse Bayesian DOA Estimation with Baseline Correction - Sparse Bayesian Learning Method with Baseline Correction [with MATLAB Code]](02.jpg)
![Sparse Bayesian DOA Estimation with Baseline Correction - Sparse Bayesian Learning Method with Baseline Correction [with MATLAB Code]](03.jpg)
![Sparse Bayesian DOA Estimation with Baseline Correction - Sparse Bayesian Learning Method with Baseline Correction [with MATLAB Code]](04.jpg)
![Sparse Bayesian DOA Estimation with Baseline Correction - Sparse Bayesian Learning Method with Baseline Correction [with MATLAB Code]](05.jpg)
![Sparse Bayesian DOA Estimation with Baseline Correction - Sparse Bayesian Learning Method with Baseline Correction [with MATLAB Code]](06.jpg)
![Sparse Bayesian DOA Estimation with Baseline Correction - Sparse Bayesian Learning Method with Baseline Correction [with MATLAB Code]](07.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
