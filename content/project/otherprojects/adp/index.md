---
title: Automatic Differetiation Ptychography
summary: Here we describe how to add a page to your site.
date: "2018-06-28T00:00:00Z"
tags: ["A Tag", "Another Tag"]
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


### Improving Acquisition Speed of X-ray Ptychography: A Concise Overview

X-ray ptychography is a pivotal technique in **nanometer resolution imaging**, offering profound insights in fields like biological imaging and material sciences. This paper unravels the potential of enhancing acquisition speed and efficiency of this technique through **spatial undersampling and regularization**.

The core of X-ray ptychography involves a coherent X-ray probe beam interacting with an object, creating an exit wavefront that is recorded on a detector. This interaction unveils intricate details of the object. However, the phase retrieval problem becomes ill-posed as the overlap between neighboring diffraction patterns reduces, posing significant challenges.

To overcome these challenges, the study explores the integration of image priors in the phase retrieval algorithm, focusing on different overlap ratios. The incorporation of image priors like **Total-Variation** and **Structure Tensor Prior** has yielded promising results, allowing for the accurate reconstruction of objects at low overlap ratios. This is particularly impactful for the reconstruction of integrated circuits (IC) from X-Ray diffraction measurements.

The extensive experimentation in this study involved simulating diffraction patterns with varying overlap ratios and utilizing the Adam optimizer. The results were enlightening, revealing the significant regularization of the solution, estimating an artifact-free object.

The real-world applicability of the proposed methods was validated using real data from an IC chip. The robustness of the algorithm was evident as it recovered most details even for very low overlap ratios when using the STP and the TV priors.

In conclusion, this paper illuminates the transformative potential of X-ray ptychography by addressing its inherent challenges through innovative regularization methods. The integration of various prior models has proven to be a game-changer, pushing the boundaries of what's possible in nanometer resolution imaging.

### Related Work
- Hoppe, W. (1969). Beugung im inhomogenen primärstrahlwellenfeld. III. Amplituden- und phasenbestimmung bei unperiodischen objekten. *Acta Crystallographica Section A: Crystal Physics, Diffraction, Theoretical and General Crystallography, 25*(4), 508–514.
- Thibault, P., Dierolf, M., Bunk, O., Menzel, A., & Pfeiffer, F. (2009). Probe retrieval in ptychographic coherent diffractive imaging. *Ultramicroscopy, 109*(4), 338–343.
- Maiden, A. M., & Rodenburg, J. M. (2009). An improved ptychographical phase retrieval algorithm for diffractive imaging. *Ultramicroscopy, 109*(10), 1256–1262.
- Kandel, S., Maddali, S., Allain, M., Hruszkewycz, S. O., Jacobsen, C., & Nashed, Y. S. G. (2019). Using automatic differentiation as a general framework for ptychographic reconstruction. *Optics Express, 27*(13), 18653–18672.