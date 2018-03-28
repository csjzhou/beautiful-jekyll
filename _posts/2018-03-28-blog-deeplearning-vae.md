---
layout: post
title:      "Variational Autoencoder: Intuition and Implementation"
subtitle:   "Variational Autoencoder (VAE) (Kingma et al., 2013) is a new perspective in the autoencoding business. It views Autoencoder as a bayesian inference problem: modeling the underlying probability distribution of data."
tags:
  - blogs
  - python
  - deeplearning
  - vae
published: true
---



From [blog](https://wiseodd.github.io/techblog/2016/12/10/variational-autoencoder/)

There are two generative models facing neck to neck in the data generation business right now: [Generative Adversarial Nets (GAN)]({% post_url 2016-09-17-gan-tensorflow %}) and Variational Autoencoder (VAE). These two models have different take on how the models are trained. GAN is rooted in game theory, its objective is to find the Nash Equilibrium between discriminator net and generator net. On the other hand, VAE is rooted in bayesian inference, i.e. it wants to model the underlying probability distribution of data so that it could sample new data from that distribution.

In this post, we will look at the intuition of VAE model and its implementation in Keras.
