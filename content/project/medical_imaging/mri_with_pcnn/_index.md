---
title: MRI PROJECT
summary: An example of linking directly to an external project website using `external_link`.
tags:
- Demo
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: http://example.org

image:
  caption: Photo by Toa Heftiba on Unsplash
  focal_point: Smart
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