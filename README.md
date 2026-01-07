# VAE for Music Genre Clustering

## Overview
This project implements an unsupervised learning pipeline using Variational Autoencoders (VAE) and Conditional VAE (CVAE) to cluster music tracks.

## Deliverables
  - **`VAE_Music_Clustering.ipynb`**: Contains the full implementation including:
  - **Easy Task**: Basic VAE, K-Means, and PCA comparison.
  - **Medium Task**: Convolutional VAE, hybrid feature representation with lyrics, and DBSCAN.
  - **Hard Task**: Conditional VAE (CVAE), NMI/Purity metrics, and reconstruction plots.
- **`requirements.txt`**: List of dependencies.

## Instructions
1. Open the `VAE_Music_Clustering.ipynb` file in Google Colab.
2. Ensure the T4 GPU is enabled.
3. Run the cells sequentially to reproduce the results.

## Note on Data
Per instructor convenience, only English tracks (GTZAN dataset) were used. OpenAI Whisper was used to generate lyrics for the hybrid representation task.

## File Structure
- `VAE_Music_Clustering.ipynb`: The main notebook containing the full pipeline (Easy, Medium, and Hard tasks).
- `requirements.txt`: List of required Python libraries.
- `results/`: Folder containing latent space visualizations and reconstruction plots.

## Implementation Details
- **Audio Processing:** Raw audio was converted to Mel-spectrograms using Librosa.
- **Lyrics:** Since the dataset lacked lyrics, OpenAI's Whisper model was used to transcribe samples for multi-modal clustering.
- **Models:** Includes a Convolutional VAE for feature extraction and a CVAE for disentangled representations.
- **Clustering:** Evaluated using K-Means, Agglomerative Clustering, and DBSCAN.

## How to Run
1. Upload `VAE_Music_Clustering.ipynb` to Google Colab.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run all cells to reproduce the results.
