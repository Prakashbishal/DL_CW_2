# Retinal OCT Classification using Deep Learning

## Overview

This project focuses on classifying retinal OCT images into four categories:

* CNV
* DME
* DRUSEN
* NORMAL

Three models were implemented and compared:

* CNN (baseline) 
* EfficientNet-B0
* Resnet50
* MobileNetV2

## Notebooks (Run in Order)

1. `01_dataset_exploration.ipynb`
2. `02_preprocessing_and_dataloaders.ipynb`
3. `03_custom_cnn.ipynb`
4. `04_resnet50.ipynb`
5. `05_efficientnet.ipynb`

---

## Results Summary

| Model                 | Test Accuracy |
| --------------------- | ------------- |
| CNN                   | ~98.45%       |
| EfficientNet-B0       | ~81.92%       |
| ResNet50              | ~85.85%       |
| MobileNetV2           | ~80.68%       |
