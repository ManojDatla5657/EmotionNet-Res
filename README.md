# Facial Emotion Recognition with ResNet152V2

This project demonstrates facial emotion recognition using the FER2013 dataset with the power of transfer learning. It leverages the pre-trained ResNet152V2 model as the base, applies data augmentation, and performs fine-tuning to achieve high accuracy on seven emotion classes.

## Project Overview

The goal of this project is to classify facial expressions into one of seven emotion categories:
- Angry
- Disgust
- Fear
- Happy
- Sad
- Surprise
- Neutral

We use the FER2013 dataset, which contains labeled images of faces showing different emotions. The model utilizes the ResNet152V2 architecture for feature extraction, combined with custom layers for emotion classification.

### Key Steps:
1. **Data Augmentation:** Enhance the dataset with random transformations (flip, shear, zoom).
2. **Pre-trained Model (ResNet152V2):** Leverage transfer learning by using ResNet152V2 pre-trained on ImageNet.
3. **Model Training:** Train the model first with frozen ResNet layers, followed by fine-tuning for improved performance.
4. **Fine-Tuning:** Unfreeze some of the final layers of ResNet152V2 to adapt the model to the emotion recognition task.

## Requirements

- Python 3.6+
- TensorFlow 2.x
- Matplotlib
- Kagglehub

## Installation

To get started with this project, first install the necessary libraries:

```bash
pip install tensorflow matplotlib kagglehub

