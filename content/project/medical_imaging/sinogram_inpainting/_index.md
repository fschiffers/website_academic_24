---
title: Enhancing Sparse-View CT Reconstruction with Neural Networks
summary: Our study introduces a pioneering two-step, domain-specific approach to enhance sparse-view CT reconstruction, employing a Sinogram Inpainting Network and a Postprocessing Refining Network coupled with a Discriminator Perceptual loss, significantly improving reconstruction quality and efficiency.

# Is this a featured talk? (true/false)
featured: false

# Link this post with a project
projects: []

# Date published
publishDate: '2017-01-01T00:00:00Z'

# url_pdf: ''
# url_code: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_dataset: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: 'https://github.com/HugoBlox/hugo-blox-builder'
# url_video: 'https://youtube.com'


image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ''
  placement: 1
  preview_only: true

# # tags:
# # - Demo
# #date: "2024-04"
# type: pages

design:
  columns: '2'
  spacing:
    # Customize the section spacing. Order is top, right, bottom, left.
    padding: ['20px', '200px', '20px', '200px']
---


<div style="text-align: left;">
   Florian Schiffers*, Haoyu Wei*, Tobias Würfl, and D. Shen, D. Kim, AK Katsaggelos, Oliver Cossairt 
</div>


<figure>
  <img src="teaser.png" alt="my alt text" style="width:50%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 1:</strong> We propose a new architecture for holographic displays specifically designed for speckle reduction. Instead of a single coherent source of illumination, our design uses a grid of multiple sources, which sum incoherently at the image plane. By using two spatial light modulators (SLMs) with an air gap in between, we break correlations between the multiple sources enabling high-resolution holograms with significantly suppressed speckle. We experimentally demonstrate speckle reduction on both 2D images (left) and focal stacks with natural defocus blur (right).
    </span>
  </figcaption>
</figure>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Paper Display</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        .paper-container table {
            width: 100%;
            border-spacing: 20px;
        }
        .paper-image img {
            width: 250px;
            height: auto;
        }
        .paper-title {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 10px;
        }
        .paper-authors {
            font-size: 16px;
            margin-bottom: 10px;
            color: #555;
        }
        .paper-conference {
            font-size: 16px;
            margin-bottom: 20px;
        }
        .paper-links {
            display: flex;
            gap: 10px;
        }
        .paper-links a {
            display: inline-block;
            padding: 5px 15px;
            text-decoration: none;
            color: #555;
            background-color: #f7f7f7;
            border: 1px solid #ddd;
            font-size: 14px;
            border-radius: 2px;
        }
        .paper-links a:hover {
            background-color: #eaeaea;
        }
        .text {
            vertical-align: top;
        }
    </style>
</head>
<body>

<div class="paper-container">
    <table>
        <tr>
            <td class="paper-image">
              <a href="paper.pdf">
                <img src="paper_thumbnail.png" alt="Paper Thumbnail" width="200px">
            </td>
            <td class="text">
                <div class="paper-title">
2-Step Sparse-View CT Reconstruction with a Domain-Specific Perceptual Network</div>
                <div class="paper-authors">
                     Florian Schiffers*, Haoyu Wei*, Tobias Würfl, and D. Shen, D. Kim, AK Katsaggelos, Oliver Cossairt 
                </div>
                <div class="paper-conference">
                    ICCP 2023
                </div>
                <div class="paper-links">
                    <a href="paper.pdf">Paper</a>
                    <a href="supplement.pdf">Supplement</a>
                    <!-- <a href="#">Bibtex</a>
                    <a href="#">Code (soon)</a> -->
                </div>
            </td>
        </tr>
    </table>
</div>
</body>
</html>
<br>

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



<figure>
  <img src="network_overview.png" alt="my alt text" style="width:100%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 1:</strong>
    </span>
  </figcaption>
</figure>


<figure>
  <img src="problem_statement.png" alt="my alt text" style="width:80%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 1:</strong>
    </span>
  </figcaption>
</figure>

<figure>
  <img src="discriminator_perceptual_loss.png" alt="my alt text" style="width:50%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 1:</strong>
    </span>
  </figcaption>
</figure>





<figure>
  <img src="result_fig_7.png" alt="my alt text" style="width:50%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 1:</strong>
    </span>
  </figcaption>
</figure>

<figure>
  <img src="results_big.png" alt="my alt text" style="width:100%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 1:</strong>
    </span>
  </figcaption>
</figure>