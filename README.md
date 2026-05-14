# Hate Speech Classification using Simple RNN

## Problem Statement

This project detects hate speech in tweets using a Simple Recurrent Neural Network (RNN).

---

## Dataset

Dataset contains:
- tweet
- label

Labels:
- 0 = Non Hate Speech
- 1 = Hate Speech

---

## Text Preprocessing

Steps performed:
- Converted text to lowercase
- Removed @mentions
- Removed URLs
- Removed special characters
- Removed numbers
- Removed extra spaces

---

## Tokenization & Vocabulary

- Tweets tokenized into words
- Vocabulary built manually
- Top 5000 words selected
- Added:
  - <PAD> token
  - <OOV> token

---

## Sequence Processing

- Converted words into integer sequences
- Applied padding
- Maximum sequence length: 25

---

## Train-Test Split

- 80% Training
- 20% Testing
- Stratified sampling used

---

## Model Architecture

Embedding Layer
↓
SimpleRNN Layer
↓
Dense Layer (Sigmoid)

---

## Training Details

- Loss Function: Binary Crossentropy
- Optimizer: Adam
- Epochs: 10
- Batch Size: 32

---

## Evaluation Metrics

- Accuracy
- F1 Score
- Confusion Matrix

---

## Final Results

Test Accuracy: XX%

F1 Score: XX%

---

## Technologies Used

- Python
- TensorFlow/Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
