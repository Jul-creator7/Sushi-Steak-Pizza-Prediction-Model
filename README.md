# Sushi, Pizza & Steak Image Classifier

A convolutional neural network built with PyTorch to classify food images into three categories:

- Sushi
- Pizza
- Steak

This project began while I was following a PyTorch deep learning course published by freeCodeCamp.org. After building the original TinyVGG-style baseline model, I continued experimenting independently with the architecture, preprocessing pipeline, and training configuration to improve its performance.

## Project Overview

The goal of this project was to gain hands-on experience building and improving an image classification model without using transfer learning.

The project includes:

- Extraction of sushi, pizza, and steak images from the Food-101 dataset
- Image preprocessing and data augmentation
- A TinyVGG-style convolutional neural network
- Training and evaluation with PyTorch
- Experiments with different model configurations
- Saved weights for the best-performing model

## Experiments

After completing the baseline model, I experimented with several changes, including:

- Increasing the number of hidden units
- Increasing input image resolution
- Modifying data augmentation
- Adding Batch Normalization
- Comparing training and test performance across different configurations

These experiments were used to select the final model configuration based on its performance on unseen test data.


## Model Performance

The best-performing configuration achieved a test accuracy of **91.20%** on the held-out test set.

This result was achieved without transfer learning, using a custom TinyVGG-style convolutional neural network trained from scratch.

## Repository Structure

```text
Sushi-Steak-Pizza-Prediction-Model/
├── models/
│   └── best_model.pth
├── notebooks/
│   ├── data_preparation.ipynb
│   └── model_experiments.ipynb
├── .gitignore
├── README.md
└── requirements.txt
```

### `notebooks/data_preparation.ipynb`

The original data preparation workflow is based on material from the freeCodeCamp.org PyTorch course.

I modified the workflow to extract all sushi, pizza, and steak images from the Food-101 dataset and organize them into the dataset used for this project.

### `notebooks/model_experiments.ipynb`

Contains the model architecture, training pipeline, evaluation process, and the experiments performed after completing the original baseline model.

### `models/best_model.pth`

Contains the saved PyTorch weights for the best-performing version of the model.

## Technologies

- Python
- PyTorch
- Torchvision
- Google Colab
- Jupyter Notebook

## Installation

Clone the repository:

```bash
git clone https://github.com/Jul-creator7/Sushi-Steak-Pizza-Prediction-Model.git
cd Sushi-Steak-Pizza-Prediction-Model
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

The notebooks can then be opened locally using Jupyter Notebook or uploaded to Google Colab.

## Live Demo

The trained model is integrated into my personal portfolio website, where users can upload an image and receive a sushi, pizza, or steak prediction.

**Portfolio:** https://julienaramouni.com

## Dataset

The images used in this project come from the Food-101 dataset.

The dataset itself is not stored in this repository. The data preparation notebook contains the workflow used to prepare the sushi, pizza, and steak subset.

## Acknowledgements

This project began while following a PyTorch deep learning course published by [freeCodeCamp.org](https://www.freecodecamp.org/).

The course provided the foundation for:

- The original data preparation workflow
- The TinyVGG-style baseline architecture
- The PyTorch training and evaluation workflow

I modified the data preparation process to extract all sushi, pizza, and steak images from Food-101. After completing the baseline model, I continued the project independently by experimenting with the architecture, preprocessing pipeline, and training configuration.

**Course:** https://www.youtube.com/watch?v=V_xro1bcAuA&t=0s

## Author

Julien Aramouni