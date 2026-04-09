# Check-damaged-car-by-computer-vision

## Overview
The goal of this project is to create an automated system that can assist insurance companies or automotive repair shops in quickly identifying vehicle damage from images.
Model Type: Convolutional Neural Network (CNN)
Library: fastai / PyTorch
Dataset: Images sourced dynamically via DuckDuckGo Search API

## Tech Stack
Python 3
fastai: For high-level deep learning abstractions.
fastcore & DuckDuckGo Search (ddgs): Used for automated image scraping.

## How It Works
1. **Data Collection
The script automatically searches for and downloads images of "damaged cars" and "clean cars" using the DuckDuckGo Search API.

2. **Training**
We use Transfer Learning with a pre-trained ResNet architecture. This allows the model to achieve high accuracy and speed even with a relatively small number of custom images.

3. **Data Cleaning**
The notebook includes an interactive ImageClassifierCleaner, allowing you to manually prune low-quality or irrelevant images from the training set to improve model robustness.

4. **Inference**
You can test the model by uploading a custom image (car.jpg). The model outputs:
Category: (e.g., "damaged car" or "not damaged")
Confidence Probability

## Getting Started
Prerequisites
Ensure you have the necessary libraries installed:

```bash
pip install -Uqq fastai ddgs fastcore
```

Running the Notebook
Clone this repository:
```bash
git clone https://github.com/nguyendkhoi/Check-damaged-car-by-computer-vision.git
```

Open the .ipynb file in Google Colab or a local Jupyter environment.

Run the cells sequentially.
