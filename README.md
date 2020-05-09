# Plagiarism Project, Machine Learning Deployment (Udacity Machine Learning Engineer)

This repository contains code and associated files for deploying a plagiarism detector using AWS SageMaker.

## Project Overview

In this project, you will be tasked with building a plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text. Detecting plagiarism is an active area of research; the task is non-trivial and the differences between paraphrased answers and original work are often not so obvious.

This project will be broken down into three main notebooks:

**Notebook 1: Data Exploration**
* Load in the corpus of plagiarism text data.
* Explore the existing data features and the data distribution.

**Notebook 2: Feature Engineering**

* Clean and pre-process the text data.
* Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Select "good" features, by analyzing the correlations between different features.
* Created Features based on 2 methods 1. Containment 2. Longest Common Subsequence
* Create train/test `.csv` files that hold the relevant features and class labels for train/test data points.

**Notebook 3: Train and Deploy Your Model in SageMaker**

* Upload your train/test feature data to S3.
* Define a binary classification model and a training script.
* Created a custom SKLearn estimator for creating the model using the training script.
* Trained binary classifer using Support Vector Machine (SVM) algorithm.
* Train your model and deploy it using SageMaker.
* Evaluate your deployed classifier.( Metrics: Accuracy, F1 Score, Precision, Recall and Confusion Matrix)



