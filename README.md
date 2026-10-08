# Image Caption Generation using CNN and LSTM

A deep learning project that automatically generates meaningful captions for images using Convolutional Neural Network (CNN) and Long Short-Term Memory (LSTM) networks.

---

## 📌 Project Overview

The objective of this project is to develop an Image Caption Generation system that can understand the visual content of an image and generate a suitable textual description.

The project combines CNN for image feature extraction and LSTM for sequence learning and caption generation.

The main steps involved in the project are:

* Image preprocessing
* CNN-based image feature extraction
* Text preprocessing
* Tokenization
* Word embedding
* LSTM-based sequence learning
* Next-word prediction
* Caption generation
* Greedy Search and Beam Search
* BLEU score evaluation

---

## 📊 Dataset

The project uses the **Flickr8K dataset**.

The dataset contains images along with their corresponding textual captions. These image-caption pairs are used to train and evaluate the image caption generation model.

### Dataset Link

Flickr8K Dataset:

https://www.kaggle.com/datasets/adityajn105/flickr8k

---

## 🧠 Model Architecture

The proposed system consists of two main deep learning components:

### 1. Convolutional Neural Network (CNN)

CNN is used to extract important visual features from the input images.

The CNN learns visual information such as:

* Objects
* Shapes
* Patterns
* People
* Animals
* Background information

The extracted visual information is represented as an image feature vector.

### 2. Long Short-Term Memory (LSTM)

LSTM is used to generate captions from the extracted image features.

The LSTM processes the caption sequence and predicts the next word step by step.

The generation process continues until the end token is produced.

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

---

## 🔧 Model Training

The CNN-LSTM model is trained using the preprocessed Flickr8K images and captions.

During training:

1. Image features are extracted using CNN.
2. Captions are tokenized and converted into numerical sequences.
3. Image features and caption sequences are provided to the model.
4. The LSTM predicts the next word.
5. The predicted word is compared with the actual word.
6. The model parameters are updated based on the prediction error.
7. The training process is repeated for multiple epochs.

---

## ✨ Caption Generation

After training, a new image is provided as input to the system.

The CNN extracts visual features from the image. The LSTM then generates the caption one word at a time.

The process starts with a start token and continues until the end token is generated or the maximum sequence length is reached.

---

## 🔍 Caption Generation Methods

The project uses two caption generation approaches:

### Greedy Search

Greedy Search selects the word with the highest probability at each prediction step.

### Beam Search

Beam Search considers multiple possible word sequences and selects a suitable overall caption sequence.

These approaches help compare different caption generation results.

---

## 📈 Model Evaluation

The generated captions are compared with the actual captions available in the dataset.

The project uses **BLEU score** to evaluate the similarity between generated captions and reference captions.

The evaluation compares:

* Actual captions
* Greedy Search generated captions
* Beam Search generated captions
* BLEU score

---

## 📊 Visualization

The project provides visualization of randomly selected test images along with their actual and generated captions.

The visualization helps to understand how effectively the model generates captions based on the visual content of the images.

---

## 📁 Project Structure

```text
Image-Caption-Generator-CNN-LSTM/
│
├── README.md
└── image-caption123.ipynb
