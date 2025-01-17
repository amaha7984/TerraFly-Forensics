# Forensic Detection Methods

## Overview
This section summarizes the results of evaluating various forensic detection methods on the TerraFly-Forensics dataset. The table below shows the classification accuracy for detecting generated images as fake, evaluating the generalization capability of each detection method when trained on one type of generative model and tested on others.

---

### Table: Cross-Generator Detection Accuracy on TerraFly-Forensics
Classification accuracy (%) for detecting generated images across different generative models. Lower accuracy indicates limited generalization capability.

| **Model**      | **Training**    | **ProGAN** | **StyleGANV2-ADA** | **LatentDiffusion**| **DiT** | **CycleGAN** | **AttentionGAN**|
|----------------|-----------------|------------|--------------------|--------------------|---------|--------------|-----------------|
| CNNSpot [1]    | DiT             | 88.75      | 63.24              | 99.09              | -       | 99.63        | 72.44           |
|                | StyleGANV2-ADA  | 60.48      | -                  | 67.36              | 4.78    | 93.88        | 84.74           |
|                | ProGAN          | -          | 49.48              | 73.68              | 17.77   | 94.44        | 77.38           |
|                | AttentionGAN    | 17.36      | 0.80               | 2.95               | 17.77   | 100.00       | -               |
|                | CycleGAN        | 3.69       | 0.40               | 61.05              | 3.75    | -            | 99.63           |
| DIRE [2]       | DiT             | 83.11      | 38.97              | 99.37              | -       | 95.73        | 62.51           |
|                | StyleGANV2-ADA  | 77.26      | -                  | 74.79              | 8.36    | 98.01        | 92.62           |
|                | ProGAN          | -          | 39.62              | 63.17              | 21.87   | 93.12        | 84.29           |
|                | AttentionGAN    | 9.70       | 0.10               | 61.60              | 17.77   | 99.92        | -               |
|                | CycleGAN        | 25.05      | 5.22               | 73.72              | 4.04    | -            | 99.88           |
| AIDE [3]       | DiT             | 66.05      | 74.03              | 92.74              | -       | 72.94        | 37.84           |
|                | StyleGANV2-ADA  | 60.26      | -                  | 96.29              | 77.92   | 96.58        | 54.55           |
|                | ProGAN          | -          | 35.92              | 94.45              | 31.63   | 42.81        | 29.80           |
|                | AttentionGAN    | 34.24      | 54.52              | 64.14              | 46.85   | 99.54        | -               |
|                | CycleGAN        | 12.21      | 20.59              | 52.73              | 42.72   | -            | 18.26           |
| RINE [4]       | DiT             | 98.20      | 99.90              | 99.80              | -       | 78.20        | 98.10           |
|                | StyleGANV2-ADA  | 99.50      | -                  | 99.90              | 84.30   | 99.70        | 99.00           |
|                | ProGAN          | -          | 89.10              | 96.80              | 82.10   | 74.30        | 95.40           |
|                | AttentionGAN    | 93.30      | 66.70              | 92.80              | 20.00   | 100.00       | -               |
|                | CycleGAN        | 91.00      | 31.80              | 89.50              | 4.70    | -            | 100.00          |

---

### References
The following forensic detection methods were evaluated on the TerraFly-Forensics dataset:

1. [Wang et al., "CNN-Generated Images Are Surprisingly Easy to Spot... for Now," CVPR 2020](https://openaccess.thecvf.com/content_CVPR_2020/papers/Wang_CNN-Generated_Images_Are_Surprisingly_Easy_to_Spot..._for_Now_CVPR_2020_paper.pdf)
2. [Wang et al., "DIRE for Diffusion-Generated Image Detection," ICCV 2023](https://openaccess.thecvf.com/content/ICCV2023/papers/Wang_DIRE_for_Diffusion-Generated_Image_Detection_ICCV_2023_paper.pdf)
3. [Yan et al., "A Sanity Check for AI-generated Image Detection," arXiv 2024](https://arxiv.org/pdf/2406.19435)
4. [Koutlis & Papadopoulos, "Leveraging Representations from Intermediate Encoder-Blocks for Synthetic Image Detection", Springer 2025](https://link.springer.com/chapter/10.1007/978-3-031-73220-1_23)
