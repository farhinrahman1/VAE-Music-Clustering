# VAE for Music Genre Clustering

## Project Overview
This project implements an unsupervised learning pipeline using Variational Autoencoders (VAE) and Conditional VAE (CVAE) to cluster music tracks from the GTZAN dataset.

## File Structure
- `GTZAN.ipynb`: The main notebook containing the full pipeline (Easy, Medium, and Hard tasks).
- `requirements.txt`: List of required Python libraries.
- `results/`: Folder containing latent space visualizations and reconstruction plots.

## Implementation Details
- **Audio Processing:** Raw audio was converted to Mel-spectrograms using Librosa.
- **Lyrics:** Since the dataset lacked lyrics, OpenAI's Whisper model was used to transcribe samples for multi-modal clustering.
- **Models:** Includes a Convolutional VAE for feature extraction and a CVAE for disentangled representations.
- **Clustering:** Evaluated using K-Means, Agglomerative Clustering, and DBSCAN.

## How to Run
1. Upload `GTZAN.ipynb` to Google Colab.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run all cells to reproduce the results.
