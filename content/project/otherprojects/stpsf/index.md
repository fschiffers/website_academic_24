---
title: Grating-Based Phase-Contrast X-Ray Tomography
summary: An example of using the in-built project page.
tags:
- Deep Learning
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

<center>{{< figure src="attenuation.png" title="Caption" >}}</center>

Talbot-Lau X-ray grating interferometry applied within a polychromatic setup suffers from additional artifacts compared to conventional attenuation imaging. Among those are beam hardening and dispersion effects due to the complex coupling of different physical effects involved in the image formation process. In computed tomography these effects lead to image degradation, such as cupping and streak artifacts, hampering diagnostic use. 

This thesis seeks to reduce these artifacts in an iterative reconstruction framework. To this purpose, we define a model of the polychromatic forward projection that includes prior knowledge about the physical setup. Using this model we derive a maximum likelihood algorithm for simultaneous reconstruction of the attenuation, phase and scatter images. 

In our experiments on a synthetic ground-truth phantom, we compare filtered back projection reconstruction with the proposed approach. The proposed method considerably reduces strong beam hardening artifacts in the phase images, and almost completely removes these artifacts in the absorption and scatter images. Reconstruction with real data has not been successful because the proposed model does not reproduce the measured reality. Further research is required to resolve this discrepancy.

Furthermore, an optimized iterative reconstruction algorithm for grating based tomography is proposed. Last, an in-depth analysis of an iterative reconstruction framework for Talbot-Lau imaging data is provided.

<figure>
<img src="example_phase_contrast.png" />
<figcaption>
<p align=”justify”>
Figure 2. Example images to demonstrate Grating Based X-Ray interferometry and the different information it provides. The specimen is made of 4 gummy bears. The first (red) was imaged without any preparation. The second (yellow) has a splinter of wood inserted on its top. The third (red) one contains pin made of metal and a plastic head. The last (white) is filled with small PMMA-beads on its top with a diameter of 6µm.
</p>
</figcaption>



<object data="IMXP_Poster.pdf" type="application/pdf" width="700px" height="900px">
    <embed src="IMXP_Poster.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="IMXP_Poster.pdf">Download PDF</a>.</p>
    </embed>
</object>

[On Computed Tomography in Talbot-Lau X-Ray Interferometry, ECAP, 2017, Masterthesis](/FlorianSchiffers_Masterthesis_2017.pdf)

[Schiffers, F., Kaeppler, S., Pelzer, G., Wolf, A., Maier, A., Anton, G., & Riess, C. Polychromatic Maximum Likelihood Reconstruction for Talbot-Lau X-ray Tomography.](/FlorianSchiffers_Fully3D2017.pdf)
