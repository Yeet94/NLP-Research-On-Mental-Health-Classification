# NLP Research on Mental Health Classification

## Overview
This research project investigates the effectiveness of Natural Language Processing (NLP) and Deep Learning techniques in classifying raw text into various mental health sentiment categories. The study explores whether advanced models like DistilBERT and BiLSTM can accurately identify mental health status from user-generated text and examines the linguistic features that distinguish these categories.

## Research Questions
1. **Model Performance:** How accurately can deep learning models (BERT/RNN) classify raw text into mental health sentiment categories compared to traditional machine learning approaches? ([Research_qs1.ipynb](Research_qs1.ipynb))
2. **Linguistic Features:** What are the most salient linguistic features (specific vocabulary, frequency of negative or passive emotional language, use of self-referential pronouns) that distinguish text associated with various mental health challenges? ([Research_qs2.ipynb](Research_qs2.ipynb))

## Dataset
The research uses the [Combined_Data.csv](Combined_Data.csv) dataset, which contains 52,681 text statements related to mental health.

**Class Distribution:**
- **Normal:** 16,343
- **Depression:** 15,404
- **Suicidal:** 10,652
- **Anxiety:** 3,841
- **Bipolar:** 2,777
- **Stress:** 2,587
- **Personality Disorder:** 1,077

## Methodology
The study evaluates four distinct models:
1. **Naive Bayes with TF-IDF:** Probabilistic baseline model.
2. **Logistic Regression with TF-IDF:** Linear baseline model with class-weight handling.
3. **BiLSTM with Word Embeddings:** RNN-based model for capturing sequential and bidirectional context.
4. **Fine-Tuned DistilBERT:** Transformer-based model leveraging transfer learning for state-of-the-art NLP performance.

**Preprocessing steps:**
- Lowercase conversion
- URL and special character removal
- Whitespace normalization
- Minimal preprocessing for BERT to preserve contextual meaning

## Key Findings
Detailed results and conclusions can be found in the [Research_Findings_and_Conclusion.ipynb] notebook.

### 1. Model Performance Hierarchy
The research established a clear performance hierarchy:
**DistilBERT > BiLSTM > Logistic Regression > Naive Bayes**

- **DistilBERT** achieved the highest accuracy and most consistent performance across all mental health categories.
- **BiLSTM** demonstrated strong contextual understanding but was occasionally outperformed by Logistic Regression on specific metrics/classes, indicating that simpler models can generalize better under certain conditions.

### 2. Feature Identification
The linguistic analysis revealed distinct patterns for different mental health states:
- **Anxiety:** Higher frequency of words like "restless" and "anxious".
- **Depression/Suicidal:** Greater usage of self-referential pronouns (e.g., "I", "me", "my") and negative sentiment markers.
- **Complex Patterns:** Deep learning models successfully captured nuanced emotional undertones and long-range dependencies that traditional models missed.

## Practical Implications
- **Mental Health Screening:** Automated assessment of patient notes or surveys for early detection.
- **Monitoring:** Continuous tracking of mental health status through text-based interactions.
- **Triage Support:** Assisting mental health services in identifying high-risk individuals.

## Ethical Considerations
- **Not a Replacement:** Models should be used as screening tools, not for professional diagnosis.
- **Privacy:** Sensitive mental health data requires strict protection and compliance (HIPAA/GDPR).
- **Bias and Fairness:** Regular auditing for demographic fairness is crucial as models may reflect biases in training data.

## Recommendations for Future Work
- **Advanced Architectures:** Exploring larger BERT variants or domain-specific models like BioBERT/MentalBERT.
- **Class Imbalance:** Implementing oversampling (SMOTE) or focal loss to improve performance on minority classes.
- **Multi-task Learning:** Joint training on related tasks like emotion detection or sentiment analysis.
- **Explainability:** Integrating tools like LIME or SHAP to provide local explanations for model predictions.

---
*Documented by Research Team*
*Status: Analysis Complete*
