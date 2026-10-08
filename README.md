# Image Caption Generation using CNN and LSTM

A deep learning project that automatically generates meaningful captions for images using a combination of Convolutional Neural Network (CNN) and Long Short-Term Memory (LSTM) networks.

---

## 📌 Project Overview

The objective of this project is to develop an Image Caption Generation system that can understand the visual content of an image and generate a suitable textual description.

The project combines:

* CNN for image feature extraction
* Text preprocessing and tokenization
* Word embedding
* LSTM for sequence learning
* Next-word prediction
* Greedy Search
* Beam Search

The CNN extracts important visual information from the image, while the LSTM uses this information to generate the caption word by word.

---

## 📊 Dataset

The project uses the **Flickr8K dataset**.

The dataset contains images along with their corresponding textual captions. These image-caption pairs are used to train the CNN-LSTM model.

### Dataset Link

Flickr8K Dataset:

https://www.kaggle.com/datasets/adityajn105/flickr8k

---

## 🧠 Model Architecture

The proposed system consists of two major deep learning components:

### 1. Convolutional Neural Network (CNN)

CNN is used to extract important visual features from the input images.

The CNN identifies information such as:

* Objects
* Shapes
* Patterns
* People
* Animals
* Background information

The extracted visual features are represented as a feature vector and provided to the caption generation network.

---

### 2. Long Short-Term Memory (LSTM)

LSTM is used to generate the caption based on the extracted image features.

The LSTM processes the caption sequence and predicts the next word step by step.

The generated caption continues until the end token is produced.

---

## 🔄 Project Workflow




```text
Input Image
     ↓
Image Preprocessing
     ↓
CNN Feature Extraction
     ↓
Image Feature Vector
     ↓
Word Embedding
     ↓
LSTM
     ↓
Next Word Prediction
     ↓
Generated Caption
---

---

## 📝 Text Preprocessing

The captions are processed before being given to the LSTM model.

The preprocessing steps include:

* Converting text into lowercase
* Removing unnecessary punctuation
* Tokenization
* Vocabulary creation
* Converting words into numerical sequences
* Adding start and end tokens
* Padding the sequences






