# Emoji Classification using RNN and LSTM

## Overview
This project aims to classify emojis based on text input using Recurrent Neural Networks (RNN) and Long Short-Term Memory (LSTM) networks. The models are trained on a dataset of text-emoji pairs and can predict the appropriate emoji for a given sentence.

## Dataset
The dataset consists of two CSV files: `train_emoji.csv` and `test_emoji.csv`. Each file contains text-emoji pairs, where the text is the input sentence and the emoji is the corresponding label.

## Model Architecture
Two models are implemented in this project:

1. **RNN Model**: 
   - Architecture: Two RNN layers with 64 units each.
   - Dropout: 0.5.

2. **LSTM Model**: 
   - Architecture: Two LSTM layers with 128 units each.
   - Dropout: 0.5.

## Training
The models are trained using the Adam optimizer and categorical cross-entropy loss. The training process involves the following steps:

1. **Data Preprocessing**: 
   - Convert words to lowercase.
   - Split sentences into words.

2. **Embedding**: 
   - Use the GloVe embedding matrix to embed words.

3. **Model Training**: 
   - Train the models on the training data for 50 epochs with a batch size of 32.

## Results
The accuracy of the models on the test data is as follows:

- **RNN Model**: 60.7%
- **LSTM Model**: 69.0%

## Prerequisites
To run this project, you will need:

- Python 3.6 or higher
- TensorFlow 2.x
- NumPy
- Pandas

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/emoji-classification.git
   cd emoji-classification
2. Install the required packages:
   ```bash
   pip install -r requirements.txt

