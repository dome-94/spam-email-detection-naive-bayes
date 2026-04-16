# Spam Email Detection Using Naive Bayes: A Comprehensive Empirical Study

## Project Overview
This project implements an end-to-end machine learning pipeline to classify emails as **Spam** or **Ham** (legitimate). Developed as part of the **MAS291 (Probability and Statistics)** course at **FPT University**, the study focuses on the practical application of Bayesian theorem and the Naive Conditional Independence assumption in natural language processing.

## Key Results
Based on an empirical evaluation using a held-out test set of **1,146 emails**, the model achieved the following performance metrics:

| Metric | Value |
| :--- | :--- |
| **Accuracy** | **97.03%** |
| **Precision** | **89.21%** |
| **Recall** | **99.63%** |
| **F1-Score** | **94.13%** |

> [cite_start]**Operational Insight:** The model prioritizes **Recall**, ensuring that nearly all spam emails (99.63%) are successfully intercepted, which is critical for security-sensitive filtering[cite: 201].

## Features & Implementation
- [cite_start]**Text Preprocessing Pipeline:** Includes lowercasing, punctuation removal, stopword filtering, and a combination of stemming and lemmatization to reduce feature sparsity[cite: 61, 71].
- [cite_start]**Probabilistic Modeling:** Implementation of the Naive Bayes algorithm using frequency-based likelihood estimation[cite: 100].
- [cite_start]**Numerical Stability:** Inference is performed in the **Log-Domain** to prevent numerical underflow during the multiplication of small probabilities[cite: 130, 131].
- [cite_start]**Independent Validation:** The model has been validated against real-world scenarios, including professional ham emails and financial scam simulations[cite: 206, 222].

## Project Structure
- `emails.csv`: The dataset containing raw email text and labels.
- `emailSpam_NaiveBayes.py`: The core Python implementation of the classifier.
- `Report.pdf`: The detailed academic report covering the mathematical derivations and error analysis.

---
**Course:** MAS291 - Probability and Statistics  
**Instructor:** Pham Thi Kim Thuy  
[cite_start]**Institution:** FPT University, Vietnam [cite: 15, 19]
