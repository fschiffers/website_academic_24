---
title: Synthethic Angiographic Fundus Imaging
summary: Here we describe how to add a page to your site.
date: "2018-06-28T00:00:00Z"
tag: ["Electronics", "Diodes"]

# View.
#   1 = List
#   2 = Compact
#   3 = Card
view: 2

# Optional header image (relative to `static/img/` folder).
header:
  caption: ""
  image: ""
---

### Introduction:
We delve into synthesizing angiographic images from conventional color fundus images using deep neural networks, aiming to provide safer diagnostic alternatives due to the potential risks associated with angiographic imaging.

### Method:
#### CycleGAN Approach:
Utilizing CycleGAN, we translate between conventional and angiographic fundus images. This model comprises generators and discriminators, trained to create images that are nearly indistinguishable from real ones. The images were preprocessed and augmented to enhance the dataset size, and the network underwent training with a learning rate that decreased over epochs.

### Results:
The synthesized images closely resembled the real angiographic images, enhancing certain structures like vessels. However, there were variations in brightness and contrast, and some small details were not accurately synthesized.

### Discussion & Future Work:
This study demonstrates the potential of using synthetic angiographic images for developing robust algorithms, but the practical utility for medical practitioners needs further exploration. Future research will focus on refining image resolution and exploring advanced data-augmentation methods.

For more insights, refer to [the paper](https://www.researchgate.net/profile/Florian-Schiffers/publication/323299238_Synthetic_Fundus_Fluorescein_Angiography_using_Deep_Neural_Networks/links/5ac2a02baca27222c75ced75/Synthetic-Fundus-Fluorescein-Angiography-using-Deep-Neural-Networks.pdf).