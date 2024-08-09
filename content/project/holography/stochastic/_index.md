---
title: Stochastic Light Field Holography
summary: An example of linking directly to an external project website using `external_link`.
tags:
- Demo
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link: https://light.princeton.edu/publication/pupil-aware-holography/![Alt text](pupil-holography.png)

image:
  caption: Photo by Toa Heftiba on Unsplash
  focal_point: Smart
  preview_only: true
---

<table>
  <tr>
    <td class="image">
        <img src="algorithm_gif-1.gif" width="8000px">
    </td>
    <td class="text">
      <a href="../project/holography/" style="text-decoration: none; color: inherit;">
        <strong>Fig. 2</strong>
        <span><em>Stochastic Light Field Holography Algorithm</em></span>
        <br>
         We wish to infer an SLM phase image φ that produces a hologram with viewable intensity matching the projections rendered from a target Light Field L. To do this, a series of pupil samples with randomly generated position, diameter, and focus, pi are passed to two equivalent image formation models: a Light Field projection operator, which produces individual target images 𝑇𝑖, and a Wigner projection operator, which produces individual output estimates 𝑇̂𝑖 for each of the pupil samples. These target and output estimates are compared using a photo-consistency loss function, which is in turn used to update the SLM phase image with a gradient descent step.
      </a>
    </td>
  </tr>
</table>