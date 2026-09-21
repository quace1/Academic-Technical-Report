# Academic Technical Reports

This repository contains selected academic technical reports authored by Vasily Yanin.

## 1. Numerical Methods for Short-Term Interest Rate Modeling and Applications to Pricing Swaps on LIBOR

**Bachelor's Thesis, National Research University Higher School of Economics, 2024**  
**Supervisor:** Jean-Francois Mehdi Jabir, PhD

This thesis studies numerical methods and parameter estimation for stochastic differential equation models of short-term interest rates.

The work considers the Vasicek, CIR, and Aït-Sahalia models and examines several numerical approximation schemes, including Euler–Maruyama, truncated Euler, tamed Euler, an implicit scheme for the CIR process, and an exponential Euler scheme. For cases in which a numerical method cannot be applied directly, transformations based on Itô's formula are used.

Model parameters are estimated using exact or approximated likelihood methods, with analytical estimators derived where possible and numerical optimization used otherwise. The resulting estimators are evaluated through simulation experiments.

The estimated CIR and Aït-Sahalia models are subsequently applied to historical LIBOR and SOFR data and to the valuation of fixed-for-floating interest-rate swaps.

**Full text:** [Bachelor's thesis PDF](./bachelor_thesis.pdf)

---

## 2. Image Editing With Diffusion Models

**Master's Thesis, National Research University Higher School of Economics, 2026**  
**Supervisor:** Aibek Alanov

This thesis studies localized text-guided image editing with pre-trained flow-based generative models. It builds on Rectified Flow, Flow Matching, and FlowEdit and formulates image editing as controlled modulation of the velocity field of a continuous-time generative model.

The main proposed method, **Spatially-Adaptive Velocity Fusion**, uses differences between source- and target-conditioned transformer attention maps to construct a spatial control signal for the prompt-induced velocity correction. Both binary hard masks and continuous soft masks are studied. The thesis also evaluates **Velocity-Gradient Correction**, an attention-free control method based on gradients of the velocity difference.

The methods are evaluated on the full public FlowEdit benchmark of **280 source-image and editing-prompt pairs** using LPIPS, CLIP Score, and HPSv2. In the reported parameter sweep, the soft-mask method reduces LPIPS from **0.2129 to 0.1246** at its strongest preservation setting, while a low-threshold hard mask improves LPIPS from **0.2129 to 0.1922** and slightly increases CLIP Score from **35.0897 to 35.1057**.

The results provide empirical evidence that attention-derived spatial signals can improve localized control of velocity-based image editing and reduce unintended changes to non-target image regions.

**Full text:** [Master's thesis PDF](./master_thesis.pdf)

**Code:** https://github.com/quace1/image_editing
