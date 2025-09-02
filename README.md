# RNN-based Part-of-Speech (POS) Tagging

This project implements a Recurrent Neural Network (RNN) for Part-of-Speech tagging, trained on a subset of the Universal Dependencies English Web Treebank (EWT) dataset. The model learns to predict the POS tag of each word in a sentence, leveraging sequential context.

---

## Features

🔤 **POS Tagging**
- RNN-based sequence model for word-level tagging  
- Handles variable-length input sequences with padding and batching  
- Supports both training and evaluation on annotated corpora  

🧾 **Data Preprocessing**
- Tokenization and vocabulary construction  
- Mapping words and tags to indices  
- Handling out-of-vocabulary (OOV) tokens  

🧠 **Model**
- Embedding layer to represent words in dense vectors  
- Recurrent hidden layers (e.g., vanilla RNN, LSTM, or GRU depending on implementation)  
- Fully connected layer for classification into POS tags  

📊 **Evaluation**
- Accuracy on held-out test data  
- Confusion matrix to analyze per-tag performance  

---

## Example

**Input sentence:**  
`The quick brown fox jumps over the lazy dog .`

**Predicted tags:**  
`DET ADJ ADJ NOUN VERB ADP DET ADJ NOUN PUNCT`

---

## Usage

1. Install dependencies:
   ```bash
   pip install torch datasets matplotlib
