# Comparing DistilBERT & DistilRoBERTa for Genre Detection

This project develops a book genre classification model that categorizes books into 32 genres using only book titles. Unlike traditional models that rely on full text, this approach demonstrates the effectiveness of leveraging concise textual information for genre detection.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Model Architecture](#model-architecture)
- [Results](#results)

## Overview

The goal of this project is to compare the performance of DistilBERT and DistilRoBERTa in classifying book genres based solely on their titles. By utilizing pre-trained transformer models, we aim to achieve high accuracy while minimizing computational resources.

## Features

- **Genre Classification**: Classify books into 32 distinct genres using only titles.
- **Model Comparison**: Evaluate the performance of DistilBERT and DistilRoBERTa.
- **Cross-Entropy Loss**: Utilized for loss calculation during training.
- **Simple Implementation**: Code is structured for easy modification and experimentation.

## Model Architecture

1. **Data Preprocessing**: Tokenization of book titles using the respective tokenizer for each model.
2. **Model Selection**:
   - **DistilBERT**: A distilled version of BERT for faster inference and lower resource usage.
   - **DistilRoBERTa**: A robust variant of DistilBERT, fine-tuned for various NLP tasks.
3. **Classification Layer**: A fully connected layer for mapping the transformer outputs to the 32 genres.
4. **Loss Function**: Cross-Entropy Loss for multi-class classification.

## Results

The models were trained and evaluated on a dataset of book titles, achieving the following accuracies:

- **DistilBERT (3 epochs)**: 70.23% accuracy
- **DistilRoBERTa (1 epoch)**: 64.3% accuracy

The results indicate that while both models perform well, DistilBERT outperforms DistilRoBERTa in this specific task when trained for a longer duration.

