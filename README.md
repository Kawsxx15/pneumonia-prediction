**Pneumonia Detection from Chest X-Rays**

-Project Overview

  This project implements and compares deep learning and hybrid models for pneumonia detection using chest X-ray images. Our approach combines state-of-the-art vision transformers (Swin Transformer, ViT, EfficientNet) with handcrafted radiomic features for robust disease prediction and model interpretability. All code, preprocessing, feature extraction, and evaluation is included for reproducibility and extension.

-**Dataset:**
  Chest X-ray & Pneumonia Dataset, available from Kaggle:

  https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

-**How It Works**

-**Data Preparation:**

  Preprocess images from the chest X-ray dataset, split into train/validation/test groups, and extract both deep and handcrafted (radiomic) features.

-**Model Training:**

  Train multiple architectures, including Swin Transformer, Vision Transformer (ViT), and EfficientNet, both as standalone and as an ensemble.

-**Ensembling**:

  Fuse predictions and radiomics using tabular ensembles to boost classification performance.

-**Interpretability:**

  Use SHAP and Grad-CAM for transparency—understanding which regions and features most impact predictions.

-**Evaluation:**

  Includes ROC curves, AUC, accuracy, and feature attribution plots for all models.

-**Important Notes**

  Note: All large model checkpoint files (e.g., .pth) and certain metrics files were removed from this repository due to their size (over 100 MB), as per GitHub's file size restrictions.
  To reproduce results, you will need to train from the code using the provided data and instructions.

-**Usage**

  Clone this repository and download the dataset from the Kaggle link above.

-**Create the environment:**

  bash

  conda env create -f environment.yml
  
  conda activate <env_name>
  
  Follow the Jupyter Notebooks and scripts for data preparation, model training, and evaluation.

-**Project Highlights**

  Hybrid Deep+Radiomic Feature Fusion for stronger generalization and interpretability.

  Comprehensive Model Comparison: Swin Transformer, Vision Transformer, EfficientNet, and ensembles.

  Strong Test Performance: Achieved up to 93% accuracy and AUC of 0.95 (ensemble).

  Clinical Transparency: Model explainability using SHAP and Grad-CAM visualizations.

  Reproducible Pipeline: Every step from data load to interpretation is included.

| This project is for research and educational purposes. Please cite the dataset authors and acknowledge this repository if using these scripts or methodology in your work. |
