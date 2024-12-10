---
layout: news
date: Now
inline: true
related_posts: false
---
My MSc Thesis Overview

My MSc thesis involved the exploration of diffusion models for super-resolution in medical imaging. Specifically Improved, Cold, and ResShift variants, with various backbones including UNet and VIT. These models were tested in both the Latent and Spatial domains, utilizing first-stage models trained in-house, such as VQVAE and VAE. Their performance was compared against established models from hugging face [MRI Autoencoder v0.1](https://huggingface.co/microsoft/mri-autoencoder-v0.1) and the [SDXL-VAE](https://huggingface.co/stabilityai/sdxl-vae).

In the in-house trained VAE, I incorporated a specialized training loss that enabled the model to converge in fewer iterations compared to the traditional combination of GAN loss, KL divergence, and pixel loss. Additionally, I experimented with LoRA to handle data from out-of-distribution sources, such as different acceleration factors in MRI images and data variations from FastMRI knee to FastMRI brain.

I plan to open-source the code and will post extensive analyses on various aspects of this work. Stay tuned for more updates on each topic.