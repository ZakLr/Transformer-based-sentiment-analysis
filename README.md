# Transformer Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-1.9%2B-orange)
![License](https://img.shields.io/badge/License-MIT-green)

This project implements a Transformer model from scratch made in one of my previous repos for sentiment analysis on the IMDb dataset. The model classifies movie reviews into **positive**, **negative**, or **neutral** sentiments. This model was made to showcase the wide use of transformers and to add some hands-on application on it

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [License](#license)
- [Contributing](#contributing)
- [Acknowledgements](#acknowledgements)

## Overview
The project includes:
- A custom Transformer model implemented in PyTorch.
- Training and evaluation scripts.
- Preprocessing and tokenization using spaCy.

In order to reduce the training time of the model, i've used a reduced version of the model architecture, i've used some small embed_size and batch_size, also i just used a small number of epochs. in order to produce better results, increase the number of hyperparams and use more computational power.

The results in my case, were an accuracy of 75% approximately and a training time of 1:30h using Google's Colab TPUs.

The dataset used in this project is the IMDB movies reviews dataset.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Transformer-Sentiment-Analysis.git
   cd Transformer-Sentiment-Analysis
   ```
2. Install the dependencies:
  ```bash
    pip install -r requirements.txt
  ```
3. Download the spaCy model:
  ```bash
    python -m spacy download en_core_web_sm
  ```
## Usage
### Training the Model

To train the Transformer model, run:
  ```bash
  python src/train.py
  ```
### Evaluating the Model

To evaluate the model on the test set, run:
  ```bash
  python src/evaluate.py
  ```
### Making Predictions

To predict the sentiment of a sentence, run:
  ```bash
  python src/predict.py --sentence "This movie was fantastic!"
  ```
## Folder Structure
```
Transformer-Sentiment-Analysis/
├── transformers_scratch.py
├── notebook.ipynb
├── saved_model
├── requirements.txt
├── LICENSE
└── README.md
```
# License

This project is licensed under the MIT License. See the LICENSE file for details.
Contributing

Contributions are welcome! Please follow these steps:

    Fork the repository.

    Create a new branch (git checkout -b feature/YourFeature).

    Commit your changes (git commit -m 'Add some feature').

    Push to the branch (git push origin feature/YourFeature).

    Open a pull request.

Acknowledgements

    PyTorch for deep learning framework.

    torchtext for dataset handling.

    spaCy for tokenization.

    IMDb Dataset for sentiment analysis.
