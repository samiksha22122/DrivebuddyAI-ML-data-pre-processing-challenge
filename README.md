# DrivebuddyAI-ML-data-pre-processing-challenge 
Pav Bhaji Image Text Classification

## Overview

The goal of this project is to train a model that can classify whether a given image is of Pav Bhaji or not. This is a text-based classification challenge, which means we will use text data from Instagram posts to determine whether the image is related to Pav Bhaji.

## Project Details

- Type: Text-Based Classification
- Technology: Python
- Libraries: scikit-learn
- Data Source: Instagram posts and images
- Dataset: `dataset.zip`
  - Contains Instagram post metadata in `pavbhaji.json`
  - Images are provided in the `images` subdirectories, categorized as '1' for Pav Bhaji and '0' for non-Pav Bhaji.

## Project Structure

The project structure is organized as follows:

```
project-root/
│
├── dataset/
│   ├── images/
│   │   ├── 1/
│   │   │   ├── [Pav Bhaji images]
│   │   ├── 0/
│   │   │   ├── [Non-Pav Bhaji images]
│   │
│   └── pavbhaji.json
│
├── your_code.py
│
├── README.md
```

## Features and Data Preprocessing

- The features for this text classification project are derived from the text data within the Instagram post metadata (`pavbhaji.json`).
- The relevant features for training the classification model include description, comments, and tags.
- Data preprocessing steps include cleaning and combining these text features, tokenizing, and using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization for feature extraction.
- The label for the classification task is binary: '1' for Pav Bhaji related posts and '0' for non-Pav Bhaji related posts.

## Model Training

- The text data features are used to train a Logistic Regression model, a commonly used algorithm for text classification tasks.
- The model is trained to predict whether the text data suggests a Pav Bhaji related image or not.

## Running the Code

1. Extract the dataset.zip file into the project directory.
2. Execute 'pavbhaji.py'.
3. The code will load and preprocess the data, train the classification model, and make predictions.


Feel free to customize this README to include any additional information specific to your project or organization. This template provides a general structure to get you started.
