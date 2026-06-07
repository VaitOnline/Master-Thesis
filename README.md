# Master's Thesis: Multiple Image Detection in Strong Lensing Systems

This repository contains the code and data analysis developed for my Master's thesis, focusing on the detection of multiple images in strong gravitational lensing systems through photometric comparison.

## 🌌 Project Overview
Strong gravitational lensing is a powerful cosmological tool, but identifying multiple images of the same background source can be challenging. This project implements a pipeline to analyze and compare the SEDs (Spectral Energy Distribution) of detected sources via a $\chi^2$-like metric. The sources are then matched with their most similar counterpart to hopefully match multiple images systems.
This project contains different parts:
1. Image processing
Loads the images, realigns them if necessary and creates a “white-light image”.
2. Detection of sources
Identifies the pixels above a certain threshold count value arbitrarily taken for source
detection, deblends, and creates a segmentation map.
3. Creation of the photometric catalog
Uses a segmentation map to create a photometric catalog containing information
about the different detected sources (position, flux, associated errors)
4. Galaxy differentiation
Separates cluster and field galaxies, defines of a zone of influence around the lens
elements, segments the reference catalog into environmental subsets.
5. Computation of similarity
Applies a SED-matching and mutual nearest neighbor (MNN) based metric to create
a dictionary ranking sources by pairwise similarity

## 🚀 Content
* `[Le_Nom_De_Ton_Notebook].ipynb` : The main Jupyter Notebook containing the data preprocessing, photometric analysis, and visualization.
* `README.md` : This documentation file.
