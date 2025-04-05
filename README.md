# Deep Learning Assignment – Autoencoders and RNNs

**Author:** Arvind Veda
**Student ID:** 700774397
**University:** University of Central Missouri  
**Course:** Neural Network & Deep Learning  

## 🔍 Overview

This project implements:
- A basic and denoising autoencoder on the MNIST dataset
- A character-level RNN for text generation using LSTM
- A sentiment classifier using RNNs on the IMDB dataset

---

## 📁 Contents

- `q1_reconstruction.png` - Visual comparison: original vs reconstructed MNIST digits
- `q2_denoising.png` - Visual comparison: noisy vs denoised images
- `q3_generated.txt` - Generated text sample from trained RNN
- `q4_report.txt` - Classification report and confusion matrix from sentiment analysis

---

## 🧠 Q1: Basic Autoencoder

- Trained a fully connected autoencoder on MNIST.
- Encoder: 784 → 32 units | Decoder: 32 → 784.
- Evaluated reconstruction quality by visualizing results.

### 🔁 Latent Dim Comparison
- Model was tested with latent sizes 16 and 64.
- Larger latent dimensions improved output clarity but increased model complexity.

---

## 🧼 Q2: Denoising Autoencoder

- Gaussian noise (mean=0, std=0.5) added to MNIST images.
- The model learns to reconstruct clean digits from noisy input.
- Useful in real-world applications like **medical imaging** (removing scanning artifacts).

---

## 📝 Q3: RNN for Text Generation

- Dataset: Shakespeare's text corpus.
- Preprocessed to create sequences of characters (one-hot encoded).
- LSTM model trained to predict the next character.
- **Temperature scaling** used for controlling randomness in text generation.

---

## 😊 Q4: Sentiment Classification (IMDB)

- Used `tensorflow.keras.datasets.imdb`.
- Preprocessed with padding and tokenization.
- Trained LSTM model to classify reviews as **positive or negative**.
- Evaluated using:
  - Confusion Matrix
  - Accuracy, Precision, Recall, F1-score

### ⚖️ Precision vs Recall
- Important for avoiding false positives in **critical applications** like product reviews, medical feedback, etc.


Git Repository Link - https://github.com/AV4397/Neural-Network_Assignement3


