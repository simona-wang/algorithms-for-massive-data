[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/simona-wang/algorithms-for-massive-data/blob/main/market_basket_analysis.ipynb)

# Market Basket Analysis

This repository contains the project developed for the **Algorithms for Massive Data** course.

The goal of the project is to perform **market-basket analysis** on the IMDb Top 1000 Movies dataset by treating each movie as a transaction (basket) and the four actors listed in the fields `Star1`, `Star2`, `Star3`, and `Star4` as items.

The objective is to discover **frequent collaborations between actors**, i.e., actor pairs that appear together in many movies.

### Dataset

IMDb Dataset of Top 1000 Movies and TV Shows  
https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows

### Repository structure 
- **market_basket_analysis.ipynb** – notebook containing the implementation and experiments  
- **report.pdf** – detailed description of the methodology and results


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

## Results 
The algorithms identify several well-known actor collaborations that frequently appear together in the dataset.

Some of the **most frequent pairs** discovered include:

- Daniel Radcliffe – Emma Watson
- Daniel Radcliffe – Rupert Grint
- Emma Watson – Rupert Grint
- Robert Downey Jr. – Chris Evans
- Harrison Ford – Carrie Fisher
- Mark Hamill – Harrison Ford

The most **frequent triples** correspond to well-known casts from popular movie series, for example:

- **Harry Potter**: Daniel Radcliffe, Emma Watson, Rupert Grint
- **Star Wars**: Mark Hamill, Harrison Ford, Carrie Fisher
- **The Lord of the Rings**: Elijah Wood, Ian McKellen, Orlando Bloom

These results confirm that the frequent itemset mining algorithms successfully capture strong collaboration patterns among actors.

## Me

Simona Wang <br>
52103A <br>
Msc in Data Science for Economics <br>
Università degli Studi di Milano
