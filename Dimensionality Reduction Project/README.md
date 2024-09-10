# Handwritten Characters Data Exploration

This project involves exploring and classifying a **custom handwritten characters dataset** using various machine learning techniques to evaluate and compare different models.

## Dataset - Custom Handwritten Characters

The dataset was generated from a set of custom characters with the following classes:  
`class_names = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', '$', '#']`.

The dataset contains 10,000 labeled images, with 1,000 examples for each class. It is divided into:
- **Training set**: 6,120 examples
- **Test set**: 2,880 examples

## Notebooks Overview

- **Training Notebook (`training.ipynb`)**: This notebook covers the data preprocessing steps, including cleaning and normalizing the images, and then proceeds to train several machine learning models. Feature extraction techniques are also explored, which are used to improve model performance.

- **Test Notebook (`test.ipynb`)**: This notebook evaluates the trained models by testing them on unseen data. It contains performance metrics and answers key questions about model performance. 

    **Important**: To ensure compatibility, the test notebook should be run in the same environment as the training notebook, particularly to maintain version consistency for libraries like `joblib`. Both notebooks were executed using Google Colab, so running them in that environment will prevent version conflicts.

All trained models, except for the final manifold model, have been pushed to this repository. The larger manifold model can be downloaded from [this link](https://drive.google.com/file/d/1ep0a5jVmbl_51DctmTqGhZ5tiYxkaE-L/view?usp=share_link).

## Report for Analysis

The accompanying IEEE-format report provides a comprehensive analysis, including:
- Detailed exploration and preprocessing techniques for the dataset.
- Model training steps and the rationale behind model selection.
- Performance evaluations and comparisons of the models.
- Final discussions and conclusions drawn from the dataset and model results.
