---
title: Grating-Based Phase-Contrast X-Ray Tomography
summary: We propose an iterative reconstruction approach to reduce artifacts, such as beam hardening and dispersion effects, in Talbot-Lau X-ray grating interferometry computed tomography by incorporating a polychromatic forward projection model that includes prior knowledge about the physical setup.
tags:
- Deep Learning
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: true

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
---


<figure>
<img src="example_phase_contrast.png" />
<figcaption>
<p align=”justify”>
<strong>Figure 1</strong>: Example images to demonstrate Grating Based X-Ray interferometry and the different information it provides. The specimen is made of 4 gummy bears. The first (red) was imaged without any preparation. The second (yellow) has a splinter of wood inserted on its top. The third (red) one contains pin made of metal and a plastic head. The last (white) is filled with small PMMA-beads on its top with a diameter of 6µm.
</p>
</figcaption>


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
Polychromatic Maximum Likelihood Reconstruction for Talbot-Lau X-ray Tomography</div>
                <div class="paper-authors">
                     Schiffers, Florian, Sebastian Kaeppler, Georg Pelzer, Andreas Wolf, Andreas Maier, Gisela Anton, and Christian Riess
                </div>
                <div class="paper-conference">
                    Fully3D 2017
                </div>
                <div class="paper-links">
                    <a href="FlorianSchiffers_Fully3D2017.pdf">Paper</a>
                    <a href="FlorianSchiffers_Masterthesis_2017.pdf">Master Thesis</a>
                    <a href="Project_Report_Tensor_Tomography.pdf">Keystone Project</a>
                    <a href="FlorianSchiffers_fully3d_presentation.pdf">Fully3D Slides</a>
                    <a href="master_thesis_presentation.pdf">Thesis Presentation Slides</a>
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


Talbot-Lau X-ray grating interferometry applied within a polychromatic setup suffers from additional artifacts compared to conventional attenuation imaging. Among those are beam hardening and dispersion effects due to the complex coupling of different physical effects involved in the image formation process. In computed tomography these effects lead to image degradation, such as cupping and streak artifacts, hampering diagnostic use. 

This thesis seeks to reduce these artifacts in an iterative reconstruction framework. To this purpose, we define a model of the polychromatic forward projection that includes prior knowledge about the physical setup. Using this model we derive a maximum likelihood algorithm for simultaneous reconstruction of the attenuation, phase and scatter images. 

In our experiments on a synthetic ground-truth phantom, we compare filtered back projection reconstruction with the proposed approach. The proposed method considerably reduces strong beam hardening artifacts in the phase images, and almost completely removes these artifacts in the absorption and scatter images. Reconstruction with real data has not been successful because the proposed model does not reproduce the measured reality. Further research is required to resolve this discrepancy.

Furthermore, an optimized iterative reconstruction algorithm for grating based tomography is proposed. Last, an in-depth analysis of an iterative reconstruction framework for Talbot-Lau imaging data is provided.





<object data="IMXP_Poster.pdf" type="application/pdf" width="700px" height="900px">
    <embed src="IMXP_Poster.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="IMXP_Poster.pdf">Download PDF</a>.</p>
    </embed>
</object>