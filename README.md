# Variational Auto-Encoder (VAE) for MNIST Dataset
Coursework part of the Course Bayesian DeepLearning (COMP0171)


## Project Overview
This project involves the development and implementation of a Variational Auto-Encoder (VAE) using PyTorch, applied on the MNIST dataset. The VAE model focuses on achieving high reconstruction accuracy and optimizing the Evidence Lower Bound (ELBO) for efficient generative modeling of image data.

## Features
- **VAE Implementation:** Custom-built Encoder and Decoder classes in PyTorch.
- **ELBO Optimization:** Function to compute and optimize the Evidence Lower Bound, enhancing model performance.
- **Data Visualization:** Tools for visualizing input images and their reconstructions.
- **Accuracy Metrics:** Evaluation of reconstruction accuracy to measure model performance.

## `ELBO_VAE` Function Overview

The `ELBO_VAE` function is a key component of the Variational Auto-Encoder model in this project. It calculates a single-sample Monte Carlo estimate of the Evidence Lower Bound (ELBO) for each data point x_i in the dataset. The ELBO is determined by the formula:

ELBO(x_i) = Expected value over q(z_i|x_i) [log(p(z_i)p(x_i|z_i)/q(z_i|x_i))]

Where:
- q(z_i|x_i) represents the conditional distribution of the latent variable z_i given the input x_i, as returned by the Encoder class.
- p(x_i|z_i) denotes the conditional distribution of the input x_i given the latent variable z_i, as returned by the Decoder class.


## Results and Metrics
- Reconstruction accuracy: 0.93
  
Input image :

![image](https://github.com/sprasadhpy/VAE_MNIST/assets/40602129/a6189302-291f-453e-8576-9a35133995df)


Reconstruction image:

![image](https://github.com/sprasadhpy/VAE_MNIST/assets/40602129/f6b72005-0d14-4ffe-8a95-3abb83f0d664)



## License
MIT

## Contact
Shyaam Prasadh , shyaam.prasadh@icloud.com

