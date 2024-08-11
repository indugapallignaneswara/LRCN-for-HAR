

# Action Recognition with Long-term Recurrent Convolutional Networks (LRCN)

This repository contains the implementation of an action recognition system using Long-term Recurrent Convolutional Networks (LRCN). The LRCN model is designed to classify human actions in videos by combining the strengths of Convolutional Neural Networks (CNNs) for spatial feature extraction and Long Short-Term Memory (LSTM) networks for temporal sequence learning.

## Overview
Action recognition is a fundamental problem in video analysis, with applications in fields such as surveillance, sports analytics, and human-computer interaction. This project leverages the LRCN architecture to accurately identify and classify different actions within video sequences.

## Features
- **LRCN Model**: Integrates CNN layers with LSTM layers to process both spatial and temporal aspects of video data.
- **Flexible Architecture**: Easy to adapt to various action recognition tasks by changing the dataset and adjusting the model parameters.
- **Preprocessing Pipeline**: Includes video frame extraction, resizing, and normalization, making the model training-ready.
- **Training and Evaluation**: Scripts to train the model and evaluate its performance on custom datasets.

## Dataset
The model is trained on a subset of the UCF101 dataset, focusing on 5 specific action categories:
- `CricketShot`
- `PlayingCello`
- `Punch`
- `ShavingBeard`
- `TennisSwing`

Each video is processed to have a resolution of 64x64 pixels and a sequence length of 16 frames.

## Model Architecture
The LRCN model architecture consists of:
- **TimeDistributed Convolutional Layers**: Extract spatial features from each video frame.
- **TimeDistributed MaxPooling and Dropout Layers**: Reduce spatial dimensions and prevent overfitting.
- **LSTM Layer**: Capture temporal dependencies between frames.
- **Dense Output Layer**: Use a softmax activation function to predict the action class.

## Getting Started

### Prerequisites
- Python 3.x
- TensorFlow or Keras

### Installation
**Clone the repository**:
    ```bash
    git clone https://github.com/indugapallignaneswara/LRCN-for-HAR.git
    ```


## Contributing
Contributions are welcome! Please open an issue or submit a pull request to contribute to the project.

