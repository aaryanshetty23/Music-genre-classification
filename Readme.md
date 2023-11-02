# Music Genre Classification Project

## Overview

This project focuses on developing machine learning models to classify music genres from audio features extracted from 3-second audio clips. The dataset includes acoustic attributes such as tempo, MFCCs, and spectral characteristics, along with genre labels for each audio clip. The goal is to build models that can accurately classify the music genres into one of several predefined categories.

## Dataset Description

The dataset consists of:
- **Audio Features**: 60 unique features extracted from 3-second audio clips.
- **Labels**: Corresponding genre labels for each audio clip.

## Objectives

1. Develop classification models using machine learning (ML) and deep learning (DL) techniques (restricted to ANN and RNN).
2. Achieve a baseline accuracy of 70%, with an acceptable range of 75% to 90%.
3. Avoid overfitting and use a good validation strategy.

## Project Structure

- `train1.csv`: Training data with audio features and genre labels.
- `test1.csv`: Test data with audio features.
- `music_genre_predictions_final.csv`: Submission file with predicted genre labels for the test set.

## Model Development

Three models were built using Artificial Neural Networks (ANN):

1. **Model 1**:
    - Layers: 128 (ReLU), Dropout (0.4), 64 (ReLU), Dropout (0.3), 10 (Softmax)
2. **Model 2**:
    - Layers: 128 (ReLU), Dropout (0.5), 64 (Leaky ReLU), Dropout (0.3), 10 (Softmax)
3. **Model 3**:
    - Layers: 128 (ReLU), Dropout (0.4), 64 (ReLU), Dropout (0.3), 10 (Softmax)

## Training and Evaluation

- **Training**: The models were trained using the Adam optimizer and sparse categorical crossentropy loss. The data was split into training and validation sets (80:20 ratio), and features were standardized.
- **Validation**: Model performance was evaluated on the validation set to ensure good generalization.
- **Testing**: Predictions were made on the test set, and accuracy was calculated by comparing predicted labels to ground truth labels.

## Usage

1. **Clone the repository**:
    ```bash
    git clone https://github.com/username/music-genre-classification.git
    cd music-genre-classification
    ```

2. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Jupyter notebook**:
    Open the Jupyter notebook and execute the cells to train the model and generate predictions.

## Results

- **Validation Accuracy**: Achieved a validation accuracy of X%.
- **Training Accuracy**: Achieved a training accuracy of Y%.
- **Test Accuracy**: Achieved a test accuracy of Z% with respect to ground truth labels.

## Conclusion

This project demonstrates the application of ANN models for music genre classification, achieving significant accuracy while avoiding overfitting through proper validation and feature standardization.
