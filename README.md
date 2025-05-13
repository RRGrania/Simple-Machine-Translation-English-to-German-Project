# Simple Machine Translation (English to German) Project

This project is a basic machine translation model from English to German using the PyTorch library. The model is based on a Sequence-to-Sequence (Seq2Seq) architecture with recurrent LSTM networks.

## Overview

This project aims to illustrate the fundamental concepts of machine translation using PyTorch. It includes the following steps:

1.  **Data Loading:** Utilizing a portion of the WMT16 English-German dataset from the Hugging Face `datasets` library.
2.  **Tokenization:** Splitting English and German texts into tokens (words and punctuation) using the SpaCy library.
3.  **Vocabulary Building:** Creating separate vocabularies for English and German based on the available data.
4.  **Encoding and Padding:** Converting tokens to numerical indices and using padding to make all sequences the same length.
5.  **Model Building:** Constructing a Seq2Seq model consisting of an Encoder and a Decoder using LSTM networks.
6.  **Training:** Training the model on the translation data using CrossEntropyLoss and the Adam optimizer.
7.  **Translation:** A simple function to translate new English sentences into German using the trained model.

## Requirements

* Python 3.x
* PyTorch
* torchdata
* torchtext
* numpy
* spacy
* `datasets` from Hugging Face
* tqdm
* collections

These libraries can be installed using pip:

```bash
pip install torch torchvision torchaudio torchdata torchtext numpy spacy datasets tqdm
python -m spacy download en_core_web_sm de_core_news_sm
