---
title: Synthethic Angiographic Fundus Imaging
summary: This study explores the use of deep learning, specifically CycleGAN, to synthesize angiographic fundus images from conventional color fundus images, aiming to provide a safer alternative to traditional angiographic imaging which carries potential risks.
date: "2018-06-28T00:00:00Z"
tag: ["Generative AI", "Deep Learning"]

# View.
#   1 = List
#   2 = Compact
#   3 = Card
view: 2

image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ''
  placement: 1
  preview_only: true
  
# Optional header image (relative to `static/img/` folder).
header:
  caption: ""
  image: ""
---


<div style="text-align: left;">
Florian Schiffers, Zekuan Yu, Steve Arguin, Andreas Maier, Qiushi Ren
</div>

<em>BVM 2018</em>


<figure>
  <img src="setup_full.png" alt="my alt text" style="width:100%"/>
  <figcaption>
    <span class="caption-text">
    <strong>Fig. 1:</strong> An intravenous, fluorescent dye bounds to leukocytes, which excites the molecules when exposed to blue light. This, in turn, produces a narrow yellow-green light. The enhanced image highlights different features of the fundus.
    </span>
  </figcaption>
</figure>


**Abstract:** Fundus fluorescein angiography yields complementary image information when compared to conventional fundus imaging. Angiographic imaging, however, may pose risks of harm to the patient. The output from both types of imaging have different characteristics, but the most prominent features of the fundus are shared in both images. Thus, the question arises if conventional fundus images alone provide enough information to synthesize an angiographic image. Our research analyzes the capacity of deep neural networks to synthesize virtual angiographic images from their conventional fundus counterparts.



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
              <a href="destination_url_here">
                <img src="paper_thumbnail.png" alt="Paper Thumbnail" width="200px">
            </td>
            <td class="text">
                <div class="paper-title">Synthetic fundus fluorescein angiography using deep neural networks</div>
                <div class="paper-authors">
                    Florian Schiffers, Zekuan Yu, Steve Arguin, Andreas Maier, Qiushi Ren
                </div>
                <div class="paper-conference">
                    BVM 2018
                </div>
                <div class="paper-links">
                    <a href="paper.pdf">Paper</a>
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
  <img src="overview.png" alt="my alt text" style="width:100%"/>
  <figcaption>
    <span class="caption-text">
    <strong>Fig. 2:</strong> The two figures visualize the composition of the loss term used for the training process of the cycleGAN architecture. <em>I<sub>F</sub></em> and <em>I<sub>C</sub></em> are the input images for the color fundus image generator <em>G<sub>C</sub></em> and the angiographic image generator <em>G<sub>F</sub></em>, respectively. Similarly, <em>D<sub>C</sub></em> and <em>D<sub>F</sub></em> denote the respective discriminator networks. Cycle consistency is enforced so that the backwards translation resembles the input image for both ways, see <em>L<sub>Cycle_Angio</sub></em> and <em>L<sub>Cycle_Color</sub></em>. The adversarial loss, i.e. the capacity of the network to distinguish between real and fake images, is modeled by <em>L<sub>DC</sub></em> and <em>L<sub>DF</sub></em>.
    </span>
  </figcaption>
</figure>


<figure>
  <img src="results.png" alt="my alt text" style="width:100%"/>
  <figcaption>
    <span class="caption-text">
     <strong>Fig. 3:</strong> Each row shows from left to right the real and generated angiographic image, the authentic color image, and the reconstructed color image to show cycle consistency. The first three rows are from dataset [10], the remaining is taken from our own data.
    </span>
  </figcaption>
</figure>




### Introduction:
We delve into synthesizing angiographic images from conventional color fundus images using deep neural networks, aiming to provide safer diagnostic alternatives due to the potential risks associated with angiographic imaging.

### Method:
#### CycleGAN Approach:
Utilizing CycleGAN, we translate between conventional and angiographic fundus images. This model comprises generators and discriminators, trained to create images that are nearly indistinguishable from real ones. The images were preprocessed and augmented to enhance the dataset size, and the network underwent training with a learning rate that decreased over epochs.

### Results:
The synthesized images closely resembled the real angiographic images, enhancing certain structures like vessels. However, there were variations in brightness and contrast, and some small details were not accurately synthesized.

### Discussion & Future Work:
This study demonstrates the potential of using synthetic angiographic images for developing robust algorithms, but the practical utility for medical practitioners needs further exploration. Future research will focus on refining image resolution and exploring advanced data-augmentation methods.



<object data="poster.pdf" type="application/pdf" width="900px" height="1200px">
    <embed src="poster.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="poster.pdf">Download PDF</a>.</p>
    </embed>
</object>