# Latent Variable Models for NLP

## Keywords 

## Overview
[Variational Inference: A Review for Statisticians (2018)]()

## Previous Work
[Latent Dirichlet Allocation (2003)]()


## Current Papers
### [Auto-encoding Variational Bayes (2014)]()
Sounds like ELBO, but it's about a reparameterization of the variational lower bound and how you can use it on iid datasets with models containing continuous latent variables

### [Neural Variational Inference for Text Processing (2016)]()
Use an autoencoder for variational inference in approximating the total posterior integral
The autoencoder serves to learn how to represent a latent variable h which is then used to determine the posterior.

### [Discovering Discrete Latent Topics with Neural Variational Inference (2017)]()
Topic modeling!
topic modeling but you don't have to pick the number of topics ???
topic modeling via backpropagation
rather than using a dirichlet prior, we teach a neural network to model the distribution of document vector distribution parameters.

### [Generating Sentences from a Continuous Space (2016)]()
treat the sentence space as a latent space, and you can draw vectors from it that incorporate better kinds of features
can perform path following to look at how sentences change in the space
problem with RNNs: word by word rather than sentence level view
not interpretable representation of global features like topic or syntax

### [Language as a Latent Variable: Discrete Generative Models for Sentence Compression (2016)]()
It's like an autoencoder for sentences, but instead of using a vector to compress the sentence, we use another sentence! This has the result of summarizing sentences.

### [A Fast Unified Model for Parsing and Sentence Understanding (2016)]()
Stack-augmented Parser-Interpreter Neural Network
removes the need for pre-parsed trees, closer to actual human processing
plus side: can do batch processing

### [Spherical Latent Spaces for Stable Variational Autoencoders (2018)]()
Instead of using Gaussian priors for p(z) in the KL term of a likelihood function, we use von Mises-Fisher distributions, which prevent KL collapse, thereby ensuring the use of a latent variable.

## Blog Posts
[Applications of Autoencoders in Natural Language Processing]()
[Blackbox and Approximate (Variational) Neural Inference]()