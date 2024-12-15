# Music Genre Classification and Similarity Analysis

## Project Overview

This project focuses on music genre classification and similarity analysis using machine learning techniques. It processes audio files, extracts relevant features, and applies various data science methods to analyze and classify music genres.

## Features

- Audio segment extraction
- Feature extraction using librosa and TIVlib
- Tabular dataset construction
- Feature analysis
- Dimensionality reduction using PCA
- Latent space analysis
- Genre-based clustering
- Similarity analysis for new songs
- Genre inference for new samples

## Requirements

- Python
- librosa
- TIVlib
- scikit-learn
- pandas
- numpy
- matplotlib

## Installation

```bash
pip install librosa tivlib scikit-learn pandas numpy matplotlib
```

## Usage

1. Prepare your dataset:
   - Organize audio files into folders by genre
   - Ensure consistent audio format (e.g., .mp3, .wav)

2. Run the main script:
   ```bash
   python music_analysis.py --data_path /path/to/your/dataset
   ```

3. Analyze the results in the output folder

## Project Structure

```
.
├── music_analysis.py
├── utils/
│   ├── audio_processing.py
│   ├── feature_extraction.py
│   └── data_analysis.py
├── models/
│   ├── dimensionality_reduction.py
│   └── clustering.py
├── data/
│   └── processed/
├── results/
│   ├── features/
│   ├── visualizations/
│   └── models/
└── README.md
```

## Workflow

1. **Audio Segment Extraction**: Load each song and select a fixed-length segment.
2. **Genre Labeling**: Save the folder name as the target feature (genre).
3. **Feature Extraction**: Extract audio features using librosa and TIVlib.
4. **Dataset Construction**: Create a tabular dataset using the extracted features.
5. **Feature Analysis**: Apply various data science methods to analyze the features.
6. **Dimensionality Reduction**: Reduce the feature space to 3D using PCA.
7. **Latent Space Analysis**: Visualize and analyze the data in the latent space.
8. **Clustering**: Cluster points in the latent space based on genre.
9. **Similarity Analysis**: Analyze how new songs relate to the training data using clustering algorithms (KNN, DBSCAN).
10. **Genre Inference**: Attempt to infer genres for new samples.

## Output

- Processed feature datasets
- Visualizations of the latent space
- Clustering results
- Similarity analysis reports
- Genre inference results for new samples
