
# Retinal OCT Classification using Deep Learning

## Overview

This project focuses on **multi-class classification of retinal OCT images** using deep learning techniques. The goal is to automatically classify scans into four categories:
**CNV, DME, DRUSEN, and NORMAL**, assisting in early diagnosis of retinal diseases.

---

## Dataset

* Source: Kaggle – *Retinal OCT Images (Optical Coherence Tomography)*
* Total samples: ~80,000 images
* Classes:

  * CNV (Choroidal Neovascularization)
  * DME (Diabetic Macular Edema)
  * DRUSEN
  * NORMAL

---

## Methodology

### 1. Preprocessing

* Image resizing (224×224)
* Normalization
* Train/Validation/Test split

### 2. Data Augmentation

* Random flips
* Rotations
* Brightness adjustments

---

## Models Used

* ResNet50 (baseline, deep architecture)
* MobileNetV2 (lightweight, efficient)

### Training Strategy

* Transfer learning (ImageNet pretrained)
* Freeze backbone → train classifier
* Fine-tune deeper layers

---

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

---

## Explainability

* Grad-CAM used to visualize model attention
* Helps verify focus on clinically relevant regions

---

## Results

* Performance compared across models
* Analysis of class-wise predictions
* Trade-off between accuracy and efficiency

---

## Challenges

* High similarity between disease classes (e.g., CNV vs DME)
* Risk of overfitting
* Need for interpretability in medical AI

---

## Conclusion

This project demonstrates the effectiveness of **transfer learning for medical image classification**, with emphasis on robust evaluation and interpretability.

---

## Future Work

* Use EfficientNet or Vision Transformers
* Improve generalization with advanced augmentation
* Explore segmentation-based approaches

---

