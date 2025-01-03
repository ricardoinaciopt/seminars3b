# UMAP Enhanced Clustering for Music Genre Classification - GROUP 1

## Project Overview

This project presents a novel approach to music genre classification using Uniform Manifold Approximation and Projection (UMAP) for dimensionality reduction and enhanced clustering. We extract a comprehensive set of audio features from music files and project them into a three-dimensional latent space, allowing for intuitive visualization and analysis of genre relationships.

## Key Features

- Extracts 20 audio features using librosa and TIV libraries
- Employs UMAP for dimensionality reduction to 3D space
- Compares supervised and pre-clustering approaches
- Provides interpretable results through 3D visualizations
- Achieves effective classification of novel, out-of-distribution samples

## Methodology

1. **Feature Extraction**: We extract spectral, rhythmic, tonal, and energy-related features from audio files using librosa and TIV libraries.

2. **Dimensionality Reduction**: UMAP is used to reduce the high-dimensional feature space to 3D, preserving both local and global structures.

3. **Clustering Approaches**:
   - Supervised: Uses target labels to guide the UMAP reduction
   - Pre-clustering: Applies k-means clustering before UMAP reduction

4. **Classification**: Nearest neighbor algorithm is used to classify new samples in the latent space.

## Dataset

We use the GTZAN "genres original" dataset, comprising 10 genres with 100 songs each, 30 seconds in length.

## Results

Our approach demonstrates effectiveness in classifying novel, out-of-distribution samples. The pre-clustering method shows better performance for music blending multiple genre elements, while the supervised approach excels for well-defined genre characteristics.

## Feature Importance

We analyze feature importance using random forest and mutual information classifiers. Top features include:

1. Onset Strength Mean
2. Percussive Variance
3. Spectral Rolloff
4. Spectral Bandwidth
5. Spectral Centroid

## Requirements

- Python 3.x
- librosa
- numpy
- pandas
- TIVlib
- scikit-learn
- UMAP-learn

## Usage

Detailed pipeline execution and code examples can be found in the accompanying Jupyter notebook.


## Acknowledgements

- librosa library: https://librosa.org/
- TIVlib: https://github.com/aframires/TIVlib
