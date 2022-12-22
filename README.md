# DLFinalProject_Fall22

This project is part of ECE-GY 7123 Deep Learning class for Fall 2022.
This implementation is inspired by the work presented in 'Modelling Context with User Embeddings for Sarcasm Detection in Social Media' (https://arxiv.org/pdf/1607.00976.pdf). The project is attempting to read between lines to detect sarcasm in political tweets. Since we are narrowing our domain and focusing on political domain, it becomes crucial for the model to know "common knowledge" in this domain to better understand the context. 

#Datasets:
  1. Political Sarcastic tweets by ETS
    https://raw.githubusercontent.com/EducationalTestingService/sarcasm/master/twitter/sarcasm_detection_shared_task_twitter_training.json
  2. News Headlines Dataset for Sarcasm Detection (collected from "TheOnion" and "HuffPost")
    https://www.kaggle.com/datasets/rmisra/news-headlines-dataset-for-sarcasm-detection?select=Sarcasm_Headlines_Dataset_v2.json
    
    To make avoid for the model to remember the training dataset and actually understand sarcasm, we have merged the above two datasets in our experimental setup. This project explores different strategies and implements 4 different Hybrid Neural Networks running on 2 different datasets. 
    
#List of Hybrid Neural Networks
  1. Word2Vec + LSTM
  2. Word2Vec + LSTM + GRU
  3. RNN + LSTM
  4. Fine tuned BERT with BertWordPieceTokenizer

All these models are implemented for both "Political Sarcastic tweets by ETS" and merged data (Political Sarcastic tweets by ETS + News Headlines Dataset for Sarcasm Detection). 
    
#System Requirements

    python 2.7
    python package gensim
    python package transformers
    python package torch
    python package tokenizers
    python package nltk
    python package tensorflow



