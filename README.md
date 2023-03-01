# Sports-Conditional Exercise Image Binary Classifier
#### By Bhavneek Singh (IIT Delhi)
#### Enroll. number: 2020EE10482
#### [Visit my portfolio!](https://bhavneek.netlify.app/)

This project is part of internship assessment test by i'm beside you. Dataset and task description was given the company itself.

## Summary
- Importing libraries, data, and pre-processing
    - Importing Libraries
    - Mounting Gdrive
    - Extracting Zip file
    - Exploring un-zipped directories
    - Pre-processing images into batches and resizing
- Approach 1: Making our own CNN
  - Initial Model (Same as tiny VGG, 82.47% Accuracy)
  - Model-2 (Increasing trainable parameters of initial, 81.30% Accuracy)
  - Training Initial model for more epochs (82.77% Accuracy)
- Approach 2.1: Transfer Learning (Feature Extraction)
  - Model 1: Resnet_v2_50 (91.72% Accuracy)
  - Model 2: Resnet_v2_152 (91.82% Accuracy)
  - Model 3: Efficientnet_B0 (92.79% Accuracy)
  - Model 4: EfficientNet_v2 (93.77% Accuracy)
  - Model 5: EfficientNetB3-sports-0.97 (67.19% Accuracy)
- Approach 2.2 Transfer Learning (Fine Tuning)
  - EfficientNetB3-sports-0.97
    - Making Layers trainable
    - Normal training data: 94.16%
    - Augmented training data: 95.72%
  - EfficientNet_v2
    - Making Layers trainable
    - Normal training data: 95.72%
    - Augmented training data: 96.69%
    - Training for more Epochs and saving checkpoint file: 97.76%
- Saving the model
