# BERT-Question_answering Transformer

This project will train a BERT-based Question Answering model with the SQuAD 2.0 dataset. It has been trained on answering questions, given a certain context, based on the ground truth answer.

Project Overview

This repository contains a Jupyter Notebook that:
1. Loads the SQuAD 2.0 dataset using `torchtext` and `datasets` library.
2. Extracts a minimum of 20 question-answer pairs for training.
3. Preprocesses the dataset into the BERT-compatible format.
4. Trains a BERT-based Question Answering (QA) model.
5. Evaluates the model's performance.
6. Performs inference to compare predicted vs. ground truth answers.

Installation
The project requires Python and dependencies such as PyTorch, Transformers, and Datasets. Install the necessary libraries before running the notebook.

Dataset
SQuAD 2.0 is used, containing passages of text, hence contexts, along with questions and their answers. The dataset is preprocessed to be in a format compatible with BERT.

Preprocessing
The dataset is tokenized using a BERT tokenizer, ensuring the model receives properly formatted inputs for training and inference.

Model Training
A pre-trained BERT model was fine-tuned on SQuAD 2.0. Appropriate training parameters are set, among them being the batch size and number of epochs.

Evaluation
The model is evaluated using standard metrics like Exact Match (EM) and F1 score to assess its accuracy in extracting answers from the provided contexts.

Inference
The trained model is used to predict answers for new questions based on given passages. The predicted answers are compared with the ground truth for validation.
