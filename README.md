# Retinal OCT Classification using Deep Learning

## Overview

This project implements deep learning models for classifying retinal OCT images into four categories:

* CNV
* DME
* DRUSEN
* NORMAL

Two approaches were explored:

* Custom CNN (baseline)
* ResNet50 with transfer learning and fine-tuning

---

## Dataset

OCT2017 dataset was used.

* Training data: split into 80% train / 20% validation
* Test data: official test set (unseen)

---

## Notebooks

Run in this order:

1. `01_dataset_exploration.ipynb`
2. `02_preprocessing_and_dataloaders.ipynb`
3. `03_custom_cnn.ipynb`
4. `04_resnet50.ipynb`

---

## Models & Results

### Custom CNN

* Test Accuracy: **93.7%**
* Limitation: Difficulty distinguishing DRUSEN from CNV

### ResNet50 (Fine-tuned)

* Test Accuracy: **98.86%**
* Significant improvement in DRUSEN classification

---

## Key Findings

* Transfer learning improves performance significantly
* Fine-tuning is essential for medical datasets
* ResNet50 reduces inter-class confusion

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
* Model checkpoints are not included

---

## Author

Harshidi Soni
MSc Artificial Intelligence
University of Southampton
