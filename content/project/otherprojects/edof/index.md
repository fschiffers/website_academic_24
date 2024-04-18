---
title: Speckle-based Super-resolution for Extended Depth-of-Field Imaging
summary: Speckle-based super-resolution is a novel computational imaging approach that enables high-resolution imaging over an extended depth-of-field by leveraging a sequence of speckle-illuminated low-resolution images.
date: "2018-06-28T00:00:00Z"
tag: "tag"
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

This project explores a novel approach for achieving high-resolution imaging over an extended depth-of-field by leveraging projected speckle patterns. In conventional imaging systems, there is a fundamental trade-off between depth-of-field and diffraction-limited resolution. Increasing the depth-of-field by using a small aperture comes at the cost of lower resolution due to diffraction limits.

To overcome this, we propose illuminating the scene with a sequence of high-frequency speckle patterns and capturing a corresponding set of low-resolution images. Each speckle pattern encodes high-frequency information about the scene which can be computationally extracted. By combining the information from multiple speckle-illuminated images, a high-resolution image can be reconstructed without sacrificing depth-of-field.

Simulation results demonstrate the feasibility and performance of this speckle-based super-resolution approach for planar objects. The method is able to successfully recover high-frequency details that are otherwise lost in a low-resolution, extended depth-of-field image.

More details about the concept, mathematical framework, and experimental setup can be found in the full COSI 2019 conference presentation available here [link to presentation PDF].