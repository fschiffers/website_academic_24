---
title: Enhancing Sparse-View CT Reconstruction - A Two-Step, Domain-Specific Approach
summary: Here we describe how to add a page to your site.
date: "2018-06-28T00:00:00Z"
tag: ["Electronics", "Diodes"]

# View.
#   1 = List
#   2 = Compact
#   3 = Card
view: 2

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: true


# Optional header image (relative to `static/img/` folder).
header:
  caption: ""
  image: ""
---

### Title: 
Revolutionizing Sparse-View CT: A Domain-Specific, Two-Step Approach

### Introduction
We tackle the challenges in sparse-view Computed Tomography (CT) reconstruction, introducing a groundbreaking framework that enhances the quality of reconstructions from undersampled data. This work focuses on a novel two-step reconstruction approach and a domain-specific perceptual network to address the limitations of existing methods in sparse-view tomography.

### Method
#### Innovative Two-Step Approach
Our method employs a Sinogram Inpainting Network (SIN) in the first step, generating super-resolved sinograms and allowing for object reconstruction without severe streak artifacts. The second step utilizes a Postprocessing Refining Network (PRN) to refine the reconstruction by removing any remaining localized artifacts, ensuring high-quality results.

#### Discriminator Perceptual Network
We introduce a Discriminator Perceptual (DP) loss, interpreting the initial layers of a discriminator as a feature extractor. This novel approach is trained simultaneously with the generator, promoting feature-level similarity and enhancing stability in our GAN training procedure.

### Results and Discussion
Our approach demonstrates substantial improvement, achieving over 4 dB PSNR in reconstruction accuracy and effectively handling high compression ratios. The innovative domain-specific perceptual loss outperforms traditional methods in accuracy, efficiency, and memory usage.

### Conclusion
This work presents a pioneering approach for enhancing sparse-view CT reconstruction, combining a two-step method and a domain-specific perceptual network. The introduced Discriminator Perceptual loss offers a stable and efficient solution, significantly advancing the field of sparse-view CT reconstruction.

For more details and to access the code, see [the paper](https://arxiv.org/pdf/2012.04743.pdf) and visit [GitHub](https://github.com/anonyr7/Sinogram-Inpainting).