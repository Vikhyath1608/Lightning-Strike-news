# Lightning Strike Classifier

![Alt Text](https://img.freepik.com/free-vector/lightning-thunderbolt-from-thunderstorm-cloud-illustration_1441-2391.jpg)

## Table of Contents
- [About](#about)
- [Requirements](#requirements)
- [Installation](#installation)
- [Process](#Process)
  - [Training the Model](#training-the-model)
  - [Running the Extractor](#running-the-extractor)
  - [Running the Application](#running-the-application)
- [Usage Notes](#usage-notes)
- [License](#license)
- [Contact](#contact)

## About
The Lightning Strike Classifier project involves training a machine learning model to classify news articles about lightning strikes. It includes a system for extracting, storing, and displaying this information on a map, updating every 24 hours.

## Requirements
Ensure you have the following dependencies installed:
- Python packages:
  ```bash
  pip install transformers datasets scikit-learn spacy torch
  python -m spacy download en_core_web_sm
  pip install accelerate
  pip install transformers[torch]
  pip install transformers==4.41.1 accelerate==0.30.1
  pip install nlpaug
  pip install trafilatura beautifulsoup4 requests newspaper3k transformers torch feedparser psycopg2-binary folium opencage langdetect
  pip install schedule
  pip install flask

## Installation
- Clone the repository:
 ```bash
 git clone https://github.com/yourusername/lightning-strike-classifier.git
Install the required dependencies as listed in the Requirements section.
## Process
### Training the Model
- Run the training script:
  ```bash
  python Train_model/NLP_model_train.py
- Input: Dataset/Train_data.csv
- Output: rained_Model/lightning_strike_classifier2
- **Note**: The repository already contains a pre trained model. Run this step only if you need to train a new model.
