# Restaurant Review Analysis

In the age of information and digital connectivity, online reviews have become a vital source of information for consumers making choices about where to dine and spend their leisure time. Restaurants, cafes, and eateries receive feedback from customers on platforms such as Yelp, TripAdvisor, and Google Reviews, providing valuable insights into the quality of their offerings, customer service, and overall experience.

Understanding and harnessing the wealth of information embedded in these reviews is crucial for restaurant owners, managers, and marketers. This repository contains a project that explores the intricacies of restaurant reviews, from data collection to insightful analysis, with the aim of uncovering valuable trends and sentiments that can inform strategic decisions and enhance the customer experience.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Collection](#data-collection)
3. [Data Preprocessing](#data-preprocessing)
    1. [Data Cleaning](#data-cleaning)
    2. [Text Preprocessing](#text-preprocessing)
        - Tokenization
        - Stop Word Removal
        - Lemmatization
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
    1. [Statistical Summary](#statistical-summary)
    2. [Data Visualization](#data-visualization)
    3. [Histogram of Rating Distribution](#histogram-of-rating-distribution-after-outlier-removal)
5. [Building Machine Learning Models](#building-machine-learning-models)
    1. [Sentiment Analysis](#sentiment-analysis)
        - Naïve Bayes Model
        - Support Vector Machine
        - XGBoost Classifier
    2. [Topic Modeling](#topic-modeling)
6. [Insights and Discussion](#insights-and-discussion)

## Introduction

This project aims to analyze restaurant reviews from various online platforms to uncover insights into customer sentiment, trends, and key topics discussed in reviews. By understanding the sentiment and topics that emerge from these reviews, restaurant owners and marketers can make data-driven decisions to improve customer satisfaction and restaurant performance.

## Data Collection

Data collection involved sourcing restaurant reviews from multiple online platforms, including Yelp, TripAdvisor, and Google Reviews. The collected data includes textual reviews, numerical ratings, review dates, restaurant names, and cuisine categories. The data was obtained from voluntary customer contributions and API sources provided by review companies.

## Data Preprocessing

Data preprocessing was a critical step in preparing the collected restaurant review dataset for comprehensive analysis. This phase involved data cleaning, text preprocessing, and outlier removal.

### Data Cleaning

The dataset was examined for missing values, and fortunately, no missing values were found. Potential outliers in the distribution of review ratings were identified and removed to maintain data integrity.

### Text Preprocessing

Text preprocessing aimed to refine the textual content of the reviews. Several techniques were applied:

- **Tokenization**: The reviews' text was divided into individual tokens or words to enable granular analysis.

- **Stop Word Removal**: Common and insignificant words (stop words) were systematically removed to focus on essential content.

- **Lemmatization**: Words were reduced to their base or root form to maintain consistency within the text data.

These preprocessing steps ensured that the textual data was ready for in-depth exploration.

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) unveiled patterns, trends, and insights within the restaurant review dataset. Statistical summaries, data visualizations, and histograms were created to better understand the data.

### Statistical Summary

Essential metrics, including mean, median, and standard deviation, provided a quantitative overview of the numerical data.

### Data Visualization

To gain insights into the language used in the reviews, the top 20 most common words in both the "tokens" and "lemmatized_words" columns were visualized. This highlighted prevalent terms in customer reviews and provided a basis for understanding key topics.

### Histogram of Rating Distribution

A histogram displayed the distribution of ratings after outlier removal, offering insights into the distribution of customer ratings.

## Building Machine Learning Models

Machine learning techniques were applied to classify reviews into positive, negative, or neutral sentiments and to identify key topics within the reviews.

### Sentiment Analysis

Multiple machine learning models, including Naïve Bayes, Support Vector Machine, and XGBoost, were employed to classify reviews based on their sentiment. Preprocessing steps included tokenization, stop word removal, and lemmatization.

### Topic Modeling

Latent Dirichlet Allocation (LDA) was applied to identify latent topics within the reviews, enabling the categorization of reviews into respective topics based on topic distributions.

## Insights and Discussion

The sentiment analysis revealed an average accuracy of 85%, indicating effective sentiment classification. Positive reviews were most prevalent, with strong performance in identifying positive sentiments. Negative reviews often cited service issues.

Topic modeling uncovered five key topics, including "Customer Service," "Bakery and Pastries," "Cakes and Desserts," "Ice Cream and Flavors," and "Overall Experience." Food quality was central to positive reviews, while service issues were common in negative reviews.

These insights can inform strategic decisions for restaurants, such as focusing on food quality, addressing service concerns, and emphasizing affordability to enhance customer satisfaction and align marketing efforts with customer expectations.
