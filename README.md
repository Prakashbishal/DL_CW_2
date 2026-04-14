# Retinal OCT Classification using Deep Learning

## Overview

This project focuses on classifying retinal OCT images into four categories:

* CNV
* DME
* DRUSEN
* NORMAL

Three models were implemented and compared:

* Custom CNN (baseline)
* ResNet50 (fine-tuned)
* EfficientNet-B0

---

## Dataset

* OCT2017 retinal dataset
* Proper **80/20 train–validation split**
* **Official test set kept completely untouched**

---

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
| Custom CNN            | ~93.7%        |
| EfficientNet-B0       | ~92.2%        |
| ResNet50 (Fine-tuned) | **~98.8%**    |

---

## Key Observations

* Transfer learning significantly improves performance
* Fine-tuning is critical for medical image classification
* ResNet50 performs best due to deeper feature representation
* EfficientNet shows stable learning but lower performance
* DRUSEN classification is the most challenging across models

---

## Project Structure

```text
DL_CW_2/
├── notebooks/
├── outputs/
├── data/
├── requirements.txt
└── README.md
```

---

## Setup

```bash
python -m venv .venv_gpu311
.venv_gpu311\Scripts\activate
pip install -r requirements.txt
```

---

## Notes

* Dataset is not included in the repository
* Model checkpoints are excluded for size reasons

---

## Author

Harshidi Soni
MSc Artificial Intelligence
University of Southampton
