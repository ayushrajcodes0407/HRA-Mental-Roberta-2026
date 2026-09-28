Dataset README

Dataset Information

This research utilizes the Sentiment Analysis for Mental Health dataset available on Kaggle.

* Dataset Name: Sentiment Analysis for Mental Health
* Author: Suchintika Sarkar
* Source: Kaggle
* Dataset URL: https://www.kaggle.com/datasets/suchintikasarkar/sentiment-analysis-for-mental-health/data

Dataset Overview

The dataset is a curated collection of mental health–related textual statements compiled from multiple publicly available sources. Each statement is annotated with one of seven mental health categories, making the dataset suitable for multi-class text classification and sentiment analysis research. It is intended for research and educational purposes in natural language processing (NLP), mental health text classification, and machine learning. (Kaggle)

Dataset Features

The dataset contains the following attributes:

Column	Description
unique_id	Unique identifier assigned to each record
Statement	Text statement or social media post
Status (Mental Health Status)	Ground-truth class label corresponding to the statement

Mental Health Categories

The dataset consists of seven classes:

* Normal
* Depression
* Suicidal
* Anxiety
* Stress
* Bipolar
* Personality Disorder

The dataset contains over 52,000 labeled text samples collected from multiple social media and publicly available mental health datasets, providing a diverse benchmark for NLP classification tasks. (Nature)

Dataset Usage in This Research

This dataset served as the primary source of textual data for model development and evaluation. The following workflow was adopted:

* Data preprocessing and cleaning
* Text normalization
* Tokenization
* Label encoding
* Train–validation–test split
* Model training and evaluation using supervised machine learning/deep learning techniques

The dataset was used solely for academic research and experimental evaluation.

Original Data Sources

According to the dataset creator, the dataset is compiled from multiple publicly available datasets, including:

* 3k Conversations Dataset for Chatbot
* Depression Reddit Cleaned
* Human Stress Prediction
* Predicting Anxiety in Mental Health Data
* Mental Health Dataset Bipolar
* Reddit Mental Health Data
* Students Anxiety and Depression Dataset
* Suicidal Mental Health Dataset
* Suicidal Tweet Detection Dataset (Kaggle)

Citation

If you use this dataset in your research, please cite the original dataset:

Sarkar, S. Sentiment Analysis for Mental Health. Kaggle Dataset.
Available at: https://www.kaggle.com/datasets/suchintikasarkar/sentiment-analysis-for-mental-health/data

Acknowledgment

The authors sincerely acknowledge Suchintika Sarkar for creating and publicly sharing the Sentiment Analysis for Mental Health dataset on Kaggle. This publicly available dataset made it possible to conduct the experiments and evaluations presented in this research.

License

The dataset is distributed under the license specified on its Kaggle page. Users should consult the official dataset page and comply with its licensing terms before redistribution or commercial use. (Kaggle)