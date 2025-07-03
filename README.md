[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6747921.svg)](https://zenodo.org/record/6747921)
## Fluorescence image analyses <b id="f20"></b>
This repository contains image analysis scripts adapted by Sovanny Taylor from Drs. Olivia M. S. Carmo and Dezerae Cox<sup id="a1">[1](#f1)</sup>.

### Analysis software
This repo relies extensively on the following python packages: [CellPose](https://www.cellpose.org/)<sup id="a5">[5](#f5)</sup>, [napari](https://napari.org/)<sup id="a6">[6](#f6)</sup>, [scikit-image](https://scikit-image.org/)<sup id="a8">[8](#f8)</sup>

## Reproducing workflow <b id="f21"></b>
### Prerequisites
Packages required for Python scripts can be accessed in the ```environment.yml``` file. To create a new conda environment containing all packages, run ```conda create -f environment.yml```. 

### Workflow
To view analysis results, including masks and validated object classification, all processing steps are available as an open-access [Zenodo dataset](https://zenodo.org/record/15253472). To reproduce the analysis presented in the manuscript, run the ```0_data_retrieval.py``` script for the analysis workflow of interest. The data retrieval script downloads and unzips the original images along with their masks and summary tables. Analysis for the paper was conducted by running the scripts in the enumerated order. To regenerate these results yourself, run the code in the order indicated by the script number for each folder.

## Advice for use
Please check off the tick boxes with an 'x' as you go.
- [ ] clone repo from github, giving it a FAIR name on your local machine (human and machine readable)
- [ ] uncomment raw_data and results folders in gitignore 
- [ ] delete placeholder files in raw_data and results folders
- [ ] upload raw data

## Useful Resources 
Editing masks systematically before manual check using skit-images<sup id="a5">[5](#f5)</sup>. This documentation<sup id="a6">[6](#f6)</sup> outlines the major cellposeSAM changes from the 2025 update, with more general information about the model here<sup id="a7">[7](#f7)</sup>.

## References
<b id="f1">1.</b> This repository format adapted from https://github.com/ocarmo/EMP1-trafficking_PTP7-analysis [↩](#a1)

<b id="f2">2.</b> Pachitariu M, Rariden M, Stringer C. Cellpose-SAM: superhuman generalization for cellular segmentation. biorxiv. 2025; doi:10.1101/2025.04.28.651001.[↩](#a2)

<b id="f3">3.</b> Sofroniew N, Lambert T, Evans K, Nunez-Iglesias J, Winston P, Bokota G, et al. napari/napari: 0.4.9rc2. Zenodo; 2021. doi:10.5281/zenodo.4915656. [↩](#a6)
updates: napari contributors (2019). napari: a multi-dimensional image viewer for python. doi:10.5281/zenodo.3555620 [↩](#a3)

<b id="f4">4.</b> Walt S van der, Schönberger JL, Nunez-Iglesias J, Boulogne F, Warner JD, Yager N, et al. scikit-image: image processing in Python. PeerJ. 2014;2: e453. doi:10.7717/peerj.453. [↩](#a4)

<b id="f5">5.</b> https://scikit-image.org/docs/0.25.x/api/skimage.morphology.html [↩](#a5)

<b id="f6">6.</b> https://cellpose.readthedocs.io/en/latest/settings.html [↩](#a6)

<b id="f7">7.</b> https://cellpose.readthedocs.io/en/latest/ [↩](#a7)
