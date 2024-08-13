---
title: Hand-guided qualitative deflectometry with a mobile device
summary: Here we describe how to add a page to your site.
tag: ["Electronics", "Diodes"]

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
Florian Willomitzer, Chia-Kai Yeh, Vikas Gupta, William Spies, Florian Schiffers, Aggelos Katsaggelos, Marc Walton, Oliver Cossairt
</div>

<em>Optics Express 2020</em>



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
                <div class="paper-title">Multisource Holography</div>
                <div class="paper-authors">
                    Grace Kuo, Florian Schiffers, Douglas Lanman, Oliver Cossairt, Nathan Matsuda
                </div>
                <div class="paper-conference">
                    ICCP 2023
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


3D imaging methods accessible to a broad audience

This body of work introduces a series of systems that only require commodity devices such as screens, (web-) cameras, low-end tablets or mobile phones to capture high-quality 3D data: The developed “Mobile Multiview Deflectometry” system exploits screen and front camera of mobile devices for deflectometry-based measurements. It works without the need for a calibration and is optimized for specular surfaces such as stained glass artworks. To compensate for the small screen, a multi-view registration technique is applied so that large surfaces can be densely reconstructed in their entirety. The “SkinScan” sensor principle uses the same hardware components but exploits photometric stereo algorithms for the measurement of matte object surfaces such as human skin.

Applications: The project is a first step towards a universal self-calibrating measurement procedure usable by a broad audience with little to no technical imaging experience. The introduced sensor principles have great potential for cultural heritage analysis and for telemedicine or medical treatment/diagnosis in developing countries.

Jump to: [Related Talk Recording] , [Publications] , [Software] , [News and Press]
