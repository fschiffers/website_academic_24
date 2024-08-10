---
title: Simulatenous Color Holography
summary: We introduce a novel simultaneous color holography framework that generates high-quality RGB holograms using a single SLM pattern, enabling increased frame rates, reduced color fringing, and improved color fidelity in a compact optical setup.
tags:
- Demo
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).

image:
  caption: Photo by Toa Heftiba on Unsplash
  focal_point: Smart
  placement: 1
  preview_only: true
---

<div style="text-align: left;">
    Eric Markley, Nathan Matsuda, Florian Schiffers, Oliver Cossairt, Grace Kuo
</div>
<em>SIGGRAPH ASIA 2023</em>

<figure>
  <img src="teaser_01.png" alt="my alt text" style="width:100%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 5:</strong>
       <em>Focal Stack Results (Experiment)</em>:
    </span>
  </figcaption>
</figure>


We propose a novel framework for simultaneous color holography that enables the use of a single spatial light modulator (SLM) pattern for generating red-green-blue (RGB) holograms. Our approach leverages a flexible optimization-based framework that incorporates a perceptual loss function, a physics-based neural network wavefront propagator, and a camera-calibrated forward model. By optimizing the SLM pattern for simultaneous RGB illumination, we eliminate the need for sequential color illumination, resulting in a 3× increase in frame rate and the complete removal of color fringing artifacts.

Our method addresses the challenges associated with simultaneous color holography, such as depth-color ambiguity and the presence of depth replicas. We take advantage of the extended phase range of the SLM to mitigate these issues and improve hologram quality. Additionally, our perceptual loss function prioritizes low-frequency color information, aligning with the human visual system's sensitivity to color, resulting in improved color fidelity and reduced noise in the generated holograms.

Through experimental validation, we demonstrate the effectiveness of our simultaneous color holography framework on both 2D and 3D content. Our compact and simple optical setup, combined with the elimination of sequential color illumination, brings us one step closer to realizing practical color holographic displays for augmented and virtual reality applications.


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
                <div class="paper-title">Simultaneous Color Computer Generated Holography</div>
                <div class="paper-authors">
                    Eric Markley, Nathan Matsuda, Florian Schiffers, Oliver Cossairt, Grace  
                </div>
                <div class="paper-conference">
                    SIGGRAPH ASIA 2023
                </div>
                <div class="paper-links">
                    <a href="paper.pdf">Paper</a>
                    <a href="https://dl.acm.org/doi/suppl/10.1145/3610548.3618250/suppl_file/SimultaneousColorSupplement_Asia_Final.pdf">Supplement</a>
                    <!-- <a href="#">Bibtex</a>
                    <a href="#">Code (soon)</a> -->
                </div>
            </td>
        </tr>
    </table>
</div>
</body>
</html>




<figure>
  <img src="comparison.png" alt="my alt text" style="width:100%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 2:</strong>
    </span>
  </figcaption>
</figure>


<figure>
  <img src="experimental_2d_capture.png" alt="my alt text" style="width:100%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 3:</strong>
 <em>Single Source vs. Multisource (Simulation):</em>
    </span>
  </figcaption>
</figure>

<figure>
  <img src="experimental_setup.png" alt="my alt text" style="width:100%"/>
  <figcaption>
    <span class="caption-text">
      <strong>Figure 4:</strong>
    </span>
  </figcaption>
</figure>

