# Master's Thesis: Multiple Image Detection in Strong Lensing Systems

This repository contains the code and data analysis developed for my Master's thesis, focusing on the detection of multiple images in strong gravitational lensing systems through photometric comparison.

## 🌌 Project Overview
Strong gravitational lensing is a powerful cosmological tool, but identifying multiple images of the same background source can be challenging. This project implements a pipeline to analyze and compare the SEDs (Spectral Energy Distribution) of detected sources via a $\chi^2$-like metric. The sources are then matched with their most similar counterpart to identify multiple-image systems.

This project is divided into five main steps:
1. **Image processing:** Loads the images, realigns them if necessary, and creates a “white-light image”.
2. **Detection of sources:** Identifies the pixels above an arbitrary threshold count value for source detection, deblends them, and creates a segmentation map.
3. **Creation of the photometric catalog:** Uses the segmentation map to create a photometric catalog containing information about the different detected sources (position, flux, associated errors).
4. **Galaxy differentiation:** Separates cluster and field galaxies, defines a zone of influence around the lens elements, and segments the reference catalog into environmental subsets.
5. **Computation of similarity:** Applies a SED-matching and Mutual Nearest Neighbor (MNN) based metric to create a dictionary ranking sources by pairwise similarity.

## 🚀 Content
* `[Multiple_Images_Detection].ipynb` : The main Jupyter Notebook containing the complete pipeline (from data preprocessing to the final similarity ranking).
* `README.md` : This documentation file.
