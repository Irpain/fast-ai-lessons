# Is it a Bird? 
This project uses **fastai** and **DuckDuckGo Search** to build a simple image classification model that can distinguish between images of birds and non-birds (e.g., forests). 
It covers data collection, training, and inference steps.

## Table of Contents 
- [Features](#features) 
- [Setup](#setup) 
- [Usage](#usage) 
- [Step 1: Download Images](#step-1-download-images) 
- [Step 2: Train the Model](#step-2-train-the-model) 
- [Step 3: Use the Model](#step-3-use-the-model) 
- [Dependencies](#dependencies)

## Features 
 - Automatically downloads images from DuckDuckGo for both "bird" and "non-bird" categories.
 - Trains a deep learning model (ResNet18) to classify the images. 
 - Provides predictions with confidence probabilities.

## Setup 1. Clone the repository: 
```bash git clone <repository_url> cd <repository_folder> ``` 

2. Install the required Python packages: 
```bash pip install -U fastai duckduckgo_search fastdownload ``` 

3. Ensure you have a stable internet connection to fetch data.

## Usage 
### Step 1: 
Download Images - Download images for "bird" and "non-bird" categories using DuckDuckGo Search. - Save the images in their respective folders for training.

### Step 2: 
Train the Model - Use `fastai`’s `vision_learner` to train a ResNet18 model on the dataset. - Fine-tune the pre-trained model using the `fine_tune()` method.

### Step 3: 
Use the Model - Test the model on new images to determine if they are "birds" or not. - Example output: ```plaintext This is a: bird. Probability it's a bird: 0.9345 ```

## Dependencies 
- Python 3.8+ - [fastai](https://docs.fast.ai/) 
- [duckduckgo_search](https://pypi.org/project/duckduckgo-search/) 
- [Pillow](https://python-pillow.org/)