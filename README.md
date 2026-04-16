# Discovering Latent Musical Structure Using Spotify Audio Features

**Course:** CS 4412 – Data Mining  
**Student:** Afra Kurudirek  

---

##  Project Overview

This project applies data mining techniques to uncover **latent musical structure** using Spotify audio features.  

Rather than focusing on prediction, the goal is **pattern discovery and interpretation** — understanding how songs relate based on measurable acoustic characteristics such as energy, tempo, and acousticness.

The analysis explores whether meaningful groupings of songs exist and what these patterns reveal about the nature of music.

---

##  Discovery Questions

- Are there natural clusters of songs based on audio features?
- What patterns exist between discovered clusters and attributes such as popularity and explicit content?
- Are there anomalous tracks that deviate significantly from typical musical patterns?

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

---

## Methods

The analysis follows a structured data mining pipeline:
