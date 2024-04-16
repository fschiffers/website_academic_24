---
title: Revolutionizing Real-Time Cine MRI with PCNN
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

### Introduction:
We're diving into the world of real-time cine MRI, focusing on enhancing image quality for patients with arrhythmia and/or dyspnea. We introduce a novel Perceptual Complex Neural Network (PCNN) for swift and efficient reconstruction of non-Cartesian real-time cine MRI k-space data.

### Method:
#### PCNN & GPU-Accelerated CS Reconstruction:
Our PCNN, trained on complex-valued MRI signals, was compared to GPU-accelerated CS reconstruction. It incorporates a perceptual loss term to refine image details and was tested using three different residual 3D U-Nets, exploring different processing and loss functions.

### Results and Discussion:
PCNN showcased rapid reconstruction, maintaining high image quality and accuracy in left ventricular functional parameters. It achieved higher data fidelity metrics compared to CS, with strong correlation and agreement in LV ejection fractions (LVEFs) measurements.

### Conclusion:
PCNN stands out as a promising approach for reconstructing non-Cartesian real-time cine MRI k-space data, especially beneficial for patients with arrhythmia and/or dyspnea, balancing artifact suppression and temporal resolution of myocardial wall motion.

For more insights, refer to [the paper](https://myaidrive.com/asV6g2Q3hx367oyS/nbm.4405-_1_.pdf).