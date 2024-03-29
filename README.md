# Spam Filter for Quora Questions

## Project Overview
This project is a machine learning model capable of identifying spam questions on Quora. Utilizing natural language processing (NLP) techniques and pre-trained word embeddings, we seek to efficiently classify questions, enhancing the quality of content on the platform.

## Dataset
The dataset for this project is available for download [here](https://www.dropbox.com/sh/kpf9z73woodfssv/AAAw1_JIzpuVvwteJCma0xMla?dl=0). It contains a collection of Quora questions labeled for spam detection.

## Model Development
### Pre-trained Embeddings
To manage the high dimensionality of text data, we leverage GloVe word embeddings. This approach helps in reducing the computational load while retaining information. Detailed guidance on using pre-trained embeddings can be found in this [Keras blog post].

### Train/Validation Split
For effective model evaluation, we create and maintain our own train/validation splits from the provided dataset.

## Running the Project
1. Download the dataset from the provided Dropbox link.
2. Follow the instructions in `Project_Quora.ipynb` to preprocess the data, train the model, and evaluate its performance.

## Contribution
Feedback and contributions are welcome. Please feel free to fork the repository, make improvements, and submit pull requests.
