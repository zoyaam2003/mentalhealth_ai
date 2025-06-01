# Semantic Differences Between Twitter-Based Expressions of Anxiety and Depression

This project investigates how symptoms of anxiety and depression are linguistically expressed on Twitter using natural language processing (NLP) and supervised machine learning models. It aims to support early detection and ethically responsible AI in digital mental health platforms.

Developed as part of a BSc dissertation at the University of Winchester, the project features a domain-specific transformer model (MentalBERT) benchmarked against classical classifiers. The system was also evaluated for ethical robustness and generalisability across social media platforms.

---

## Project Objectives

- Analyse the semantic and temporal characteristics of social media posts related to anxiety, depression, and suicidal ideation.
- Develop AI models, including both classical and transformer-based classifiers, to detect mental health-related distress using text data from Reddit and Twitter.
- Evaluate model performance across different datasets and label categories, focusing on interpretability and recall for high-risk classes like suicide.
- Address ethical considerations, including algorithmic bias, data privacy, and the implications of misclassification in mental health contexts.
- Propose practical applications of NLP-based mental health screening tools, while acknowledging the limitations of deploying them in real-world scenarios without clinical oversight.

---

## Project Structure
mentalhealth_ai/
- Data Cleaning + MentalBERT Model.ipynb: Handles data preprocessing and transformer model training.

- Logistic Regression + TF-IDF.ipynb: Implements a classical machine learning baseline using logistic regression.

- MentalBERT + Post Processing Adjustments.ipynb: Applies final tweaks and performance tuning to the MentalBERT model.

- Random Forest + TF-IDF for Multi-label.ipynb: Uses a classical ensemble approach with Random Forest for multi-label classification.

- SVM + TF-IDF for Multi-label Mental Health.ipynb: Employs an SVM classifier for multi-label mental health prediction.

- README.md: Provides an overview of the project and documentation.

---

## Models Implemented

| Model              | Type          | Description |
|-------------------|---------------|-------------|
| Logistic Regression | Classical ML | Baseline classifier using TF-IDF features |
| SVM                | Classical ML | Handles high-dimensional sparse data |
| Random Forest      | Classical ML | Non-linear ensemble with good generalisation |
| **MentalBERT**     | Transformer   | Fine-tuned BERT model using Reddit mental health data |

---

## Project Results

- **MentalBERT** achieved the highest macro-F1 score across datasets.
- Post-processing boosted recall, especially for high-risk labels like *suicidal ideation*.
- Temporal and linguistic variations between Reddit and Twitter were visualised using Power BI.

---

## Data Sources

- **Reddit**: r/Depression, r/Anxiety, r/SuicideWatch, r/CasualConversations (via AcademicTorrents)
- **Twitter**: Kaggle mental health tweet datasets, including suicidal ideation posts

> *Note: Raw data is not included due to licensing restrictions.*

---

## Tools & Libraries Used

- Python 3.10
- HuggingFace Transformers
- Scikit-learn
- Pandas / Numpy
- PyTorch

---

## Citation

> Aamir, Z. (2025). *AI-Driven Detection of Mental Health Signals on Social Media: Semantic, Temporal, and Ethical Perspectives*. Undergraduate Dissertation, University of Winchester.
