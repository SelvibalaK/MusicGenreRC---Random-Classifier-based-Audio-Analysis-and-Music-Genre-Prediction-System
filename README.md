# MusicGenreRC---Random-Classifier-based-Audio-Analysis-and-Music-Genre-Prediction-System
## Overview
This project implements a music genre classification system using a random classifier approach. Unlike the previous deep learning model, which utilized Mel spectrogram images as a dataset, this approach is based on extracting MFCC (Mel-Frequency Cepstral Coefficients) features from audio files to improve efficiency and accuracy.

## Dataset
The dataset is sourced from the GTZAN dataset, a well-known dataset in the music genre classification domain, containing:

Genres Original: A collection of 10 genres, each with 100 audio files, all 30 seconds long.
CSV Files: Two files containing feature measurements:
The first file includes the mean and variance of various features computed over each 30-second audio file.
The second file has the same structure, but the songs are split into 3-second segments, increasing the amount of data available for classification.
For more details and to download the dataset, visit: Kaggle GTZAN Dataset.

## Motivation
The primary motivation for this approach was to reduce training time and memory consumption compared to the deep learning method while achieving reasonable accuracy.

## Features
* Utilizes a random forest classifier to predict music genres based on MFCC features.
* Allows users to input their own audio files for genre prediction.
* Achieved an accuracy of 76% on the test data.

## Installation
### Prerequisites
Ensure you have the following libraries installed:
bash
pip install pandas numpy scikit-learn librosa

### Instructions
1. Download the GTZAN dataset from the provided link.
2. Place the features_30_sec.csv file in your project directory.
3. Upload the provided Python script directly to your environment (e.g., Jupyter Notebook).

### Running the Project
1. Load the dataset
2. Run the classification code
3.. Use the predict_genre function to predict the genre of your own audio files

## Evaluation
The model's performance is evaluated using accuracy and a classification report that provides precision, recall, and F1-score metrics for each genre.

## Development
This project is complete and is a standalone implementation. Contributions and feedback are welcome!

## License
This project is licensed under the MIT License.

