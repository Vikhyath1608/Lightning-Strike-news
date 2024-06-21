# Lightning Strike Classifier

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

##Process
### Training the Model
