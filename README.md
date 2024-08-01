# Aspect Based Sentiment Analysis on Google Reviews for Bobobox
This repository contains a project focused on Aspect Based Sentiment Analysis (ABSA) of Google Reviews for Bobobox. The project consists of four main stages: Scraping, Preprocessing, Modeling, and Grouping Aspects.

## Table of Contents
- [Introduction](#introduction)
- [Scraping](#scraping)
- [Preprocessing](#Process)
- [Modeling](#Modeling)
- [Grouping Aspects](#GroupingAspects)
- [Results](#results)
- [Usage](#Usage)
- [Contributing](#Contributing)

## Introduction
In this project, we perform Aspect Based Sentiment Analysis on Google Reviews for 34 Bobobox locations, including 17 Bobocabin and 17 Bobopod branches. The goal is to extract aspects from reviews and analyze the sentiment associated with each aspect.

## Scraping
For the scraping process, we collected reviews from Google Maps for each of the 34 Bobobox locations using BeautifulSoup and Selenium. The reviews were gathered and stored in a structured format for further processing.

## Preprocessing
The preprocessing stage involved several steps to clean and prepare the data for analysis:

- Combining data from multiple sources
- Dropping missing values
- Converting text to lowercase
- Normalizing slang terms
- Translating text to English using Google Translate
- Removing emojis and punctuation
- Singularizing text

## Modeling
For aspect extraction and sentiment analysis, we used the DeBERTa v3 model. The process involved:
- Extracting aspects from the review text
- Analyzing the sentiment for each extracted aspect
  
## Grouping Aspects
After extracting and analyzing aspects, we found around 2000 distinct aspects. To simplify analysis, we grouped these aspects into 8 main topics using GloVe embeddings. This involved mapping each aspect to the closest predefined aspect category.

## Results
The analysis resulted in the identification of key aspects and their associated sentiments from Google Reviews of Bobobox locations. Grouping these aspects into main topics provided a clearer understanding of customer feedback.

## Usage
To run the code and reproduce the results, follow these steps:

1. Clone this repository:
   ```shell
   git clone https://github.com/harunasrori/bobobox_reviews.git
   ```

