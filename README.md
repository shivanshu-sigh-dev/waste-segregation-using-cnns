# Waste Material Segregation Using CNNs

## Overview

This project implements an automated waste material segregation system using Convolutional Neural Networks (CNNs). The goal is to accurately classify waste images into distinct categories, thereby improving recycling efficiency, reducing landfill waste, and promoting sustainable waste management practices.

## Objectives

- Accurately classify waste materials into categories such as Cardboard, Food Waste, Glass, Metal, Other, Paper, and Plastic.
- Enhance waste segregation efficiency to support recycling and reduce environmental pollution.
- Leverage deep learning techniques to optimize sorting methods for sustainability.

## Dataset

- The dataset consists of images organized into 7 categories: Cardboard, Food Waste, Glass, Metal, Other, Paper, and Plastic.
- Images are stored in separate folders for each class.
- There is a class imbalance, with some categories having fewer images.
- Images vary in size and are resized to a consistent shape for model input.

## Approach

1. **Data Preparation**
    - Images are loaded, resized, and normalized.
    - Labels are encoded for model training.
    - Data visualization is performed to understand class distribution and sample images.

2. **Data Augmentation**
    - Augmentation techniques (random flip, rotation, zoom, contrast, brightness) are applied to increase data diversity and balance classes.

3. **Model Building**
    - A CNN with 3 convolutional layers, batch normalization, dropout, and fully connected layers is built.
    - Early stopping and model checkpointing are used to prevent overfitting.

4. **Training and Evaluation**
    - The model is trained on the processed dataset.
    - Performance is evaluated using accuracy, loss, classification report, and confusion matrix.

## Results

- Data augmentation and class balancing significantly improved model performance, especially for minority classes.
- The final model achieved high validation accuracy and low loss (e.g., Validation Accuracy: 0.92, Validation Loss: 0.23).
- The model demonstrated strong generalization and effective distinction between waste types.

## Insights

- Data augmentation is crucial for handling class imbalance and improving model robustness.
- The CNN-based approach supports automated waste segregation, aiding sustainable waste management.
- Further improvements can be achieved by exploring advanced architectures or expanding the dataset.

## Getting Started

1. **Clone the repository**
    ```bash
    git clone https://github.com/yourusername/waste-segregation-using-cnns.git
    cd waste-segregation-using-cnns
    ```

2. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3. **Prepare the dataset**
    - Place the dataset in the `data/` directory, organized by class folders.

4. **Run the notebook**
    - Open `CNN_Assg_Waste_Segregation_Starter.ipynb` in Jupyter or VS Code and follow the steps.

## Requirements

- Python 3.12
- TensorFlow
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
- Pillow

Install all dependencies using:
```bash
pip install -r requirements.txt