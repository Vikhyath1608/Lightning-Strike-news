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

### Running the Extractor
- To extract and update the database:
  ```bash
  python scheduler.py
- This will trigger Main.py every 24 hours and update the database.
- Input: Trained_Model/lightning_strike_classifier2, Input/Input_rss.csv
- Output: Database/news_data.db
- **Note** : The database already contains extracted content. Run this step only if the database needs to be updated.

### Running the Application
- To run the web application:
  ```bash
  python app.py 
- Input: Database/news_data.db
- Output: Rendered HTML page displayed at
  ```bash
  http://127.0.0.1:5000
  
## Usage Notes
- To directly run the application, use:
  ```bash
  python app.py
- To train the model, use:
  ```bash
  python Train_model/NLP_model_train.py
- To update the Database manually, use:
  ```bash
  python Main.py
- To automatically update the database every 24 hours, use:
  ```bash
  python scheduler.py

## Contact
- For support or inquiries:
Email: vikhyathraims0109@gmail.com
