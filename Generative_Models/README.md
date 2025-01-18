# Generative Models

## Quantitative Comparison of Generative Models

### Table: Quantitative comparison of FID and KID scores across various models for map generation
Lower scores indicate better performance.

| **Model**                 | **FID ↓**  | **KID (Mean ± Std) ↓**     |
|---------------------------|------------|----------------------------|
| ProGAN [1]                | 104.3720   | 0.0709 ± 0.0018            |
| StyleGANV2-ADA [2]        | 38.0042    | 0.0215 ± 0.0011            |
| LatentDiffusion [3]       | 73.6138    | 0.0573 ± 0.0025            |
| DiT [4]                   | 62.4027    | 0.0362 ± 0.0018            |
| CycleGAN [5]              | 41.6488    | 0.0251 ± 0.0013            |
| AttentionGAN [6]          | 39.5313    | 0.0237 ± 0.0013            |

---

### References
1. Karras et al., "Progressive Growing of GANs for Improved Quality, Stability, and Variation," 2017. [Link](https://arxiv.org/abs/1710.10196)  
2. Karras et al., "Training Generative Adversarial Networks with Limited Data," 2020. [Link](https://arxiv.org/abs/2006.06676)  
3. Rombach et al., "High-Resolution Image Synthesis with Latent Diffusion Models," 2022. [Link](https://arxiv.org/abs/2112.10752)  
4. Peebles et al., "Scalable Diffusion Models with Transformers," 2023. [Link](https://arxiv.org/abs/2212.09748)  
5. Zhu et al., "Unpaired Image-to-Image Translation Using Cycle-Consistent Adversarial Networks," 2017. [Link](https://arxiv.org/abs/1703.10593)  
6. Tang et al., "AttentionGAN: Unpaired Image-to-Image Translation Using Attention-Guided Generative Adversarial Networks," 2021. [Link](https://arxiv.org/abs/1911.11897)
