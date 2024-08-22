---
title: TODO - MRI with PCNN
cms_exclude: true

# View.
#   1 = List
#   2 = Compact
#   3 = Card
#   4 = Citation
view: 2

# Optional header image (relative to `static/media/` folder).
banner:
  caption: ''
  image: ''

image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: true


design:
  columns: '1'
  spacing:
    # Customize the section spacing. Order is top, right, bottom, left.
    padding: ['0px', '200px', '0px', '200px']
---
<div style="text-align: left;">
   Hui Lin, Santiago López-Tapia, Florian Schiffers, Y. Wu, S. Gunasekaran, J. Hwang, D. Bishara, E. Kholmovski, M. Elbaz, RS. Passman, Daniel Kim, and Aggelos K. Katsaggelos
</div>

<em>Heliyon 2024</em>

<table>
  <tr>
      <td class="image">
        <img src="header.png" width="2500px">
    </td>
        <td class="text">
      <a href="../project/holography/" style="text-decoration: none; color: inherit;">
<p><strong>Fig. 1.</strong> The proposed Usformer belonging to single 3D methods captures the inter-slice correlation not included in the 2D methods and avoids error propagation introduced in two-stage methods.</p>
    </td>
  </tr>
</table>



**Abstract**: Left atrial (LA) fibrosis significantly influences the progression of atrial fibrillation, with 3D late gadolinium-enhancement (LGE) MRI being a proven method for identifying LA fibrosis. However, manual segmentation of the LA wall from 3D LGE MRI is time-consuming and difficult. Automated segmentation is also challenging due to varying data intensities, limited contrast between the LA and surrounding tissues, and the complex anatomy of the LA. Traditional 3D network approaches are computationally intensive, often requiring two-stage methods. To address these issues, we propose Usformer, a lightweight, transformer-based 3D architecture for precise, single-stage LA segmentation. Usformer’s transposed attention captures global context efficiently, outperforming state-of-the-art methods in both accuracy and speed, with a dice score of 93.1% in the 2018 Atrial Segmentation Challenge and 92.0% on our local dataset. Usformer also significantly reduces parameter count and computational complexity by 2.8x and 3.8x, respectively, and achieves a 92.1% dice score using only 16 labeled MRI scans. This method may enhance the clinical translation of LA LGE for catheter ablation planning in atrial fibrillation.

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
            width: 550px;
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
                <img src="paper_thumbnail.png" alt="Paper Thumbnail" width="400px">
            </td>
            <td class="text">
                <div class="paper-title">Usformer: A small network for left atrium segmentation of 3D LGE
MRI</div>
                <div class="paper-authors">
                Hui Lin, Santiago López-Tapia, Florian Schiffers, Y. Wu, S. Gunasekaran, J. Hwang, D. Bishara, E. Kholmovski, M. Elbaz, RS. Passman, Daniel Kim, and Aggelos K. Katsaggelos
                </div>
                <div class="paper-conference">
                    Heliyon 2024
                </div>
                <div class="paper-links">
                    <a href="paper.pdf">Paper</a>
                    <!-- <a href="supplement.pdf">Supplement</a> -->
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





<figure>
  <img src="architecture.png" alt="my alt text" style="width:80%"/>
  <figcaption>
    <span class="caption-text">
<p><strong>Fig. 2.</strong> The architecture of Usformer. It is designed for end-to-end left atrium segmentation from 3D LGE MRIs. In the final two stages, the U-Net architecture integrates transformer blocks represented by the orange boxes. The transposed block includes both a transposed attention module (shown in Fig. 3) and a feed-forward network made up of fully connected layers. <i>H × W × Ż</i> represents the size of a 3D LGE scan. All feature maps are 3D volumes instead of 2D images. For additional insights into Usformer, please turn to Section 2.</p>
    </span>
  </figcaption>
</figure>




<table>
  <tr>
    <td class="text">
      <a href="../project/holography/" style="text-decoration: none; color: inherit;">
<p><strong>Fig. 3.</strong> Transformer attention module, where the matrix K is transposed to significantly decrease computation complexity. The output of the transposed attention is calculated by Equation (1). <i>Ĥ × Ŵ × Ż</i> represent the input size, and the variable <i>n</i> represents the total number of voxels present in the input, which is calculated as <i>Ĥ × Ŵ × Ż</i>, much larger than the channel number <i>Ĉ</i>. The computation complexity of the transposed module is <i>O(n<sup>2</sup>Ĉ)</i>, much smaller than the conventional module’s <i>O(Ĉ<sup>2</sup>n)</i>.</p>
    </td>
      <td class="image">
        <img src="usformer_block.png" width="1500px">
    </td>
  </tr>
</table>


<table>
  <tr>
    <td class="text">
      <a href="../project/holography/" style="text-decoration: none; color: inherit;">
<p><strong>Fig. 4.</strong> Example 3D LGE MRIs in the challenge and NU datasets with manual segmentations denoted in orange. Each slice of the LGE MRI scans underwent manual segmentation, and the resulting results were aggregated to construct a 3D model of the left atrium. Viewing this figure in color is advised in the printed edition for optimal visualization.</p>
    </td>
      <td class="image">
        <img src="example_dataset.png" width="2500px">
    </td>
  </tr>
</table>


<figure>
  <img src="results_la_segmentation_axial_view.png" alt="my alt text" style="width:90%"/>
  <figcaption>
    <span class="caption-text">
<p><strong>Fig. 6.</strong> Results of LA segmentation in the axial view by Usformer, nnU-Net [10], UNeXt [36], and TMS-Net [35]. Cases are randomly selected from the challenge and NU datasets, respectively. Each visualization includes the 2D dice score, denoted in the top left corner. Red and green delineate the contours of manual and predicted segmentation. Arrows highlight regions where Usformer exhibits notably superior performance in comparison to the other two baselines. Viewing this figure in color is advised in the printed edition.</p>
    </span>
  </figcaption>
</figure>


<table>
  <tr>
      <td class="image">
        <img src="results_3d_graphics.png" width="5500px">
    </td>
    <td class="text">
      <a href="../project/holography/" style="text-decoration: none; color: inherit;">
<p><strong>Fig. 7.</strong> Three-dimensional representation of the best, median, and worst left atrium segmentation implemented by our method regarding the 3D dice score. The first and second columns are from the challenge and NU datasets, respectively. Distance from the manual segmentation to the prediction is indicated by the color of the surface. For improved visualization, the surface distances are rescaled within the range of 0 to 10 mm. Arrows (1) and (2) highlight the errors in MV and PV, respectively. Viewing this figure in color is advised in the printed edition.</p>
    </td>
  </tr>
</table>
