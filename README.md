# Yield Curve Autoencoders

This repository contains the code and model implementations from my master's thesis:  
**"Autoencoders for Yield Curve Modelling"**, University of Copenhagen, 2025.

The project explores various neural network architectures for yield curve reconstruction, including:
- Pure (unconstrained) autoencoders
- Arbitrage-minimizing models
- Arbitrage-free affine models (with 3 ODE solvers)
- A quadratic extension
- An HJM-based arbitrage-minimizing model

## 📁 Repository Structure

- `BloombergData/` – Raw data files exported from Bloomberg
- `Data/` – Processed data used for model training and evaluation
- `README.md` – Overview and instructions for this repository

### 🔧 Notebooks

Each model and configuration is implemented in a dedicated Jupyter notebook:

- **Pure Autoencoder**
  - `pure_autoencoder_2_factor.ipynb`
  - `pure_autoencoder_3_factor.ipynb`

- **Arbitrage-Minimizing Autoencoder**
  - `arbitrage_minimizing_autoencoder_2_factor.ipynb`
  - `arbitrage_minimizing_autoencoder_3_factor.ipynb`

- **Arbitrage-Free Affine Autoencoder**
  - Constant method:
    - `arbitrage_free_affine_autoencoder_constant_method_2_factor.ipynb`
    - `arbitrage_free_affine_autoencoder_constant_method_3_factor.ipynb`
  - Constant interpolation:
    - `arbitrage_free_affine_autoencoder_constant_interpolation_2_factor.ipynb`
    - `arbitrage_free_affine_autoencoder_constant_interpolation_3_factor.ipynb`
  - Linear interpolation:
    - `arbitrage_free_affine_autoencoder_linear_interpolation_2_factor.ipynb`
    - `arbitrage_free_affine_autoencoder_linear_interpolation_3_factor.ipynb`

- **Quadratic Extension**
  - `arbitrage_free_quadratic_autoencoder_linear_interpolation_2_factor.ipynb`

- **HJM-Based Arbitrage-Minimizing Autoencoder**
  - `HJM.ipynb`
