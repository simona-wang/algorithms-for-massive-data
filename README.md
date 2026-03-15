# Market Basket Analysis

This repository contains the project developed for the **Algorithms for Massive Data** course.

The goal of the project is to perform **market-basket analysis** on the IMDb Top 1000 Movies dataset by treating each movie as a transaction (basket) and the four actors listed in the fields `Star1`, `Star2`, `Star3`, and `Star4` as items.

The objective is to discover **frequent collaborations between actors**, i.e., actor pairs that appear together in many movies.


### Dataset

IMDb Dataset of Top 1000 Movies and TV Shows  
https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows

## Implemented Algorithms

The notebook implements and compares three frequent itemset mining algorithms:

**Apriori**
- Baseline algorithm for frequent itemset mining.
- Generates candidate pairs from frequent singletons and counts their support.

**PCY (Park–Chen–Yu)**
- Optimization of Apriori using hash buckets.
- Reduces the number of candidate pairs through bucket-based pruning.

**SON (Savasere–Omiecinski–Navathe)**
- Partition-based algorithm designed for distributed environments.
- Finds candidate pairs locally in partitions and verifies them globally.

## Content of the notebook

- Data Loading & Preprocessing 
- Algorithms implementation
- A-Priori vs PCY
- Scalability experiments on increasing dataset size

## Open the Notebook in Google Colab

Click below to run the notebook directly in Google Colab.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/YOUR_REPO/blob/main/market_basket_analysis.ipynb)
