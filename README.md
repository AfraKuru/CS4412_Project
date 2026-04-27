# Discovering Latent Musical Structure Using Spotify Audio Features

**Course:** CS 4412 – Data Mining  
**Student:** Afra Kurudirek  

---

##  Project Overview

This project applies data mining techniques to uncover latent musical structure using Spotify audio features.

Rather than focusing on prediction, the goal is pattern discovery and interpretation—understanding how songs relate based on measurable acoustic characteristics such as energy, tempo, and acousticness.

The central objective is to explore whether meaningful groupings of songs exist and what these patterns reveal about the nature of music as a system.

---

##  Discovery Questions

This project is guided by three key questions:
- Are there natural clusters of songs based on audio features?
- What patterns exist between discovered clusters and attributes such as popularity and explicit content?
- Are there anomalous tracks that deviate significantly from typical musical patterns?

The emphasis is on unsupervised learning and interpretation, not prediction.
---

##  Dataset

**Spotify Tracks Dataset (Kaggle)**  
https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset  

**Dataset Details:**
- ~114,000 tracks  
- 21 features  
- ~45 MB  

**Key Features:**
- Danceability (0–1): suitability for dancing  
- Energy (0–1): intensity of the track  
- Loudness (dB): overall volume  
- Acousticness (0–1): likelihood of acoustic sound  
- Valence (0–1): musical positivity  
- Tempo (BPM): speed of the track  

The dataset is clean with minimal missing values and no duplicates, making it well-suited for unsupervised learning.

## Data Quality
- Only 3 missing values (metadata)
- No duplicates
- Clean numerical features

The dataset is well-suited for unsupervised learning techniques.

---

## Methods

The analysis follows a structured data mining pipeline:

1. Data Preprocessing
  - Removed non-informative features
  - Handled missing values
  - Standardized features using Z-score normalization
2. Dimensionality Reduction
  - Principal Component Analysis (PCA)
  - Used for visualization and structure discovery
3. Clustering
  - K-Means Clustering
    - Identifies global patterns
    - Optimal k determined using Elbow Method and Silhouette Score
  - DBSCAN
    - Detects density-based clusters and noise
4. Anomaly Detection
  - Local Outlier Factor (LOF)
    - Identifies unusual or rare tracks
5. Evaluation
  - Silhouette Score
  - Visual inspection (PCA projections)
  - Cluster interpretation
