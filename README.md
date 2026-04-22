# Arabic Dialect Classification

This project focuses on **Arabic dialect identification** using Natural Language Processing (NLP) techniques on the **SADA dataset**.  
It compares classical machine learning and transformer-based approaches for classifying Arabic dialects from text.

## Overview

Arabic dialect classification is a challenging task because Arabic varies significantly across regions such as Najdi, Hijazi, Khaliji, Egyptian, Levantine, and others.  
In this project, we trained and evaluated three different models:

- **Logistic Regression** with TF-IDF
- **AraBERT**
- **MARBERT**

The goal was to determine which model performs best on Arabic dialect classification and to analyze the effect of preprocessing and class imbalance on performance.

## Dataset

The project uses the **SADA 2022 dataset**, which contains Arabic text samples labeled by dialect.

Selected columns:
- `GroundTruthText` → input text
- `SpeakerDialect` → target label

## Preprocessing

A custom preprocessing pipeline was applied to Arabic text, including:

- Text normalization
- Diacritics removal
- Noise and punctuation removal
- Removal of English characters and symbols
- Tokenization
- Stop word removal
- Repeated character handling

## Models

### 1. Logistic Regression
A baseline machine learning model trained using **TF-IDF** features.

### 2. AraBERT
A transformer-based Arabic language model fine-tuned for dialect classification.

### 3. MARBERT
A transformer model designed for dialectal Arabic and social media text.

## Results

| Model | Accuracy | Macro F1 | Macro Recall |
|------|----------|----------|--------------|
| AraBERT | 55.7% | 0.249 | 0.238 |
| MARBERT | 56.7% | 0.258 | 0.246 |
| Logistic Regression (weighted) | 43.0% | 0.20 | 0.33 |

## Tools and Technologies

- Python
- Google Colab
- Scikit-learn
- Hugging Face Transformers
- PyTorch
- Pandas
- NLTK
- Matplotlib
- Seaborn

## Project Structure

```bash
arabic-dialect-classification/
├── README.md
├── notebooks/
├── reports/
├── images/
├── src/
└── requirements.txt
Key Findings
MARBERT achieved the best overall performance.
AraBERT showed strong results, especially on more formal Arabic text.
Logistic Regression was a useful baseline and improved minority-class recall when class balancing was applied.
Class imbalance was one of the main challenges in this task.
Future Work
Data augmentation for low-resource dialects
Audio-text multimodal classification
Hyperparameter tuning
Cross-validation
Ensemble learning
Explainability using SHAP or LIME
Authors
Ruba Alfageeh
Shahad Almutairi
Tala Melaih
Safaa Alsufyani
Supervisor
Dr. Roshayu Mohammed
