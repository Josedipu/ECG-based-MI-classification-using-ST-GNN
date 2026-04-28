# ECG-Based Myocardial Infarction Severity Classification

This project presents a deep learning-based framework for **Myocardial Infarction (MI) severity classification** using 12-lead ECG signals. It was developed as a final-year research project to improve automated cardiac diagnosis by combining signal preprocessing with a Spatio-Temporal Graph Neural Network (ST-GNN) model.

## Overview

Cardiovascular diseases require early and reliable diagnosis, and ECG remains one of the most accessible non-invasive tools for this purpose. This project focuses on analyzing multi-lead ECG signals to classify MI severity more accurately by modeling both temporal patterns and inter-lead relationships.

Unlike conventional single-stream deep learning approaches, this work uses an ST-GNN architecture to capture spatial dependencies among ECG leads along with time-varying signal characteristics. The system was evaluated in a patient-independent setting to improve robustness and generalization.

## Objectives

- Build a 12-lead ECG processing pipeline for MI severity classification.
- Reduce ECG noise and improve signal quality before model inference.
- Capture both spatial and temporal dependencies using an ST-GNN model.
- Benchmark the proposed approach against baseline models such as CNN-LSTM and attention-based RNN architectures.
- Achieve reliable classification performance suitable for intelligent healthcare applications.

## Methodology

### 1. ECG Preprocessing

The raw ECG signals are first passed through a preprocessing pipeline to improve data quality and remove unwanted artifacts. This stage includes wavelet denoising, adaptive LMS filtering, and 125 Hz windowing for cleaner and more informative feature extraction.

### 2. Feature Learning

After preprocessing, the model learns patterns from 12-lead ECG recordings using a Spatio-Temporal Graph Neural Network. This allows the framework to model both the correlation between different ECG leads and the time-dependent dynamics of cardiac activity.

### 3. Model Evaluation

The proposed model was benchmarked against CNN-LSTM and attention-based RNN baselines. Evaluation was performed in patient-independent settings, where the ST-GNN model demonstrated stronger diagnostic performance across the evaluated metrics.

## Key Features

- 12-lead ECG signal analysis.
- Wavelet denoising for noise suppression.
- Adaptive LMS filtering for signal enhancement.
- 125 Hz window-based preprocessing pipeline.
- Spatio-Temporal Graph Neural Network for multi-lead representation learning.
- Patient-independent model evaluation.
- Comparison with CNN-LSTM and attention-based RNN baselines.

## Results

The project achieved **above 90% classification accuracy** for MI severity classification. The ST-GNN-based approach outperformed the baseline deep learning models across the evaluated performance metrics, showing the benefit of graph-based modeling for multi-lead ECG interpretation.

## Technologies Used

- Python
- TensorFlow
- Digital Signal Processing (DSP) techniques
- Graph Neural Networks
- Machine Learning / Deep Learning workflows
