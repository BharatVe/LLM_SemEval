# Emotion Detection and Intensity Prediction

## **Project Overview**
This repository is for our project as part of **SemEval 2025 Task 11-A**, focusing on **emotion detection** and **intensity prediction** from text. The goal is to classify emotions expressed in a text snippet and predict their intensity. The target emotions include:

- **Joy**
- **Sadness**
- **Fear**
- **Anger**
- **Surprise**
- **Disgust**

This project involves multi-label classification and ordinal intensity prediction for a single language (English).

---

## **Goals**
1. Develop a machine learning model capable of:
   - Detecting multiple emotions in a text.
   - Predicting the intensity of each detected emotion.
2. Focus on a single-language (English) dataset to optimize accuracy.
3. Provide explainability and insights into the model's predictions using tools like SHAP.
4. Evaluate the model's performance using the **F-score** and explore comparisons with human judgments.

---

## **Tasks**
1. Preprocess and explore the dataset to prepare it for model training.
2. Fine-tune transformer models (e.g., **RoBERTa**) for:
   - Emotion detection (multi-label classification).
   - Intensity prediction (ordinal regression or classification).
3. Conduct model evaluation and error analysis.
4. Perform explainability analysis to interpret the model's predictions.
5. Document findings, results, and challenges.

---

## **Dataset Specifications**
- **Source**: Dataset provided by the SemEval 2025 Task 11-A competition (download from Codabench).
- **Language**: English.
- **Structure**: Text snippets with labels for emotions and optional intensity levels.
- **Emotion Classes**: Joy, sadness, fear, anger, surprise, disgust.
- **Intensity Levels**: 
  - 0: No emotion.
  - 1: Low intensity.
  - 2: Moderate intensity.
  - 3: High intensity.



## **Outline of Plan**

### **Phase 1: Data Preparation**
- Download and preprocess the dataset.
- Explore label distributions and handle class imbalance.
- Tokenize text using RoBERTa's tokenizer.

### **Phase 2: Model Development**
- Fine-tune **RoBERTa** for emotion detection and intensity prediction.
- Add dual-output heads:
  - Multi-label classification for emotions.
  - Ordinal regression or classification for intensity.

### **Phase 3: Evaluation**
- Evaluate the model using:
  - F-score for emotion detection.
  - Mean Squared Error or Weighted F-score for intensity.
- Compare results with baseline models.

### **Phase 4: Explainability**
- Use SHAP to analyze model predictions and identify key text features contributing to emotions and intensity.

### **Phase 5: Deployment and Reporting**
- Develop APIs for emotion and intensity prediction.
- Document the model's performance, insights, and challenges.
- Prepare a final report for submission.

---

## **Getting Started**
### **Dependencies**
- Python 3.8+
- Hugging Face Transformers
- PyTorch or TensorFlow
- SHAP for explainability

### **To Do**
- Set up the repository structure.
- Collaborate on preprocessing scripts and baseline models.
- Divide tasks among team members for efficient progress.

---

### **Links**
- [SemEval 2025 Task 11-A Details](https://www.codabench.org/competitions/3863/)
- [Competition GitHub Repository](https://github.com/emotion-analysis-project/SemEval2025-Task11)
- [BERT Text Classification Tutorial](https://www.tensorflow.org/text/tutorials/classify_text_with_bert)
- [RoBERTa Explanation](https://medium.com/@hugmanskj/hands-on-head-based-text-classification-with-bert-0a1775d5db9d)
- [SHAP for Text Analysis](https://shap.readthedocs.io/en/latest/example_notebooks/text_examples/sentiment_analysis/Emotion%20classification%20multiclass%20example.html)

---
