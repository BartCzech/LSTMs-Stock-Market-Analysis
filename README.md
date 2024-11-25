# Stock Market Analysis with Machine Learning

This repository contains a series of Jupyter Notebooks created as part of my bachelor thesis titled **"Application of Machine Learning Algorithms for Stock Market Instrument Analysis."** The project focuses on applying machine learning techniques, particularly Long Short-Term Memory (LSTM) models, for stock market prediction. It also incorporates sentiment analysis to explore the relationship between public sentiment and stock price trends, as well as statistical methods (RSI, EMA).

Through this project, I explore the challenges and possibilities of leveraging the aforementioned methods. The work highlights key insights, trends, and limitations of these approaches, but also numerous pitfalls which many novice ML developers often fall into, misinterpreting model outputs as highly accurate predictions.

---

## Repository Overview

The repository is structured into five notebooks, each covering a specific aspect of the workflow:

### 1. **Data Collecting**
   - Development of a web scraping bot to extract article text, publication dates, and URLs from [Financial Post](https://business.financialpost.com).
   - Collection of historical stock price data for selected companies from Yahoo! Finance.
   - Outputs:
     - News datasets in `.csv` and `.pkl` formats containing articles, publication dates, and links.
     - Historical price data in `.pkl` format.
   - Visualizes historical stock prices for better understanding of the datasets.

---

### 2. **Sentiment Analysis**
   - Sentiment analysis of news articles using VADER (Valence Aware Dictionary and sEntiment Reasoner), a lexicon- and rule-based NLP tool designed for sentiment analysis of textual data.
   - Comparing VADER against BERT (Bidirectional encoder representations from transformers) and FinBERT
   - Visualization of sentiment trends alongside stock prices.
   - Key Observations:
     - Does the sentiment align well with stock prices?
     - Are investors relying on sentiment-driven (fundamental) analysis rather than market price data (technical) analysis?
   - Highlights the potential of price and sentiment data for short-term trading and medium-term investing.

---

### 3. **LSTM Basic Price Prediction**
   - Demonstrates a basic LSTM model for stock price prediction using a sliding window approach. 
   - Key Findings:
     - LSTM predictions closely follow actual price trends. What is wrong with such an approach?
   - Introduces recursive predictions for forecasting the next 50 days.
   - Outlines two potential paths forward:
     1. Predict daily price changes rather than actual prices.
     2. Capture long-term trends to aid investment decisions.

---

### 4. **LSTM Next-Day Returns**
   - Integration of sentiment and price data for next-day returns prediction (short-term trading).
   - Key Features:
     - Use of statistical indicators (e.g., RSI) and price differences for returns prediction.
     - Binary classification (price up or down).
     - Incorporation of sentiment analysis to assess its impact on predictions.
   - Allows users to experiment with model features and parameters to evaluate their effectiveness.

---

### 5. **LSTM - Trend Prediction**
   - Explores the potential of LSTM models for predicting general price trends over the next X days instead of daily price movements
   - Key Question: Can LSTMs effectively identify broad market trends, making them useful for long-term (30-90 days) investment strategies?
   - Useful charts comparing the investment strategy against the actual stock returns.

---

## Highlights of the Project
- **Comprehensive Workflow**: Covers the complete process from data collection and sentiment analysis to advanced LSTM-based predictions.
- **Innovative Insights**: Explores the interplay between fundamental and technical analysis, highlighting post-2020 trends in investor behavior.
- **Practical Applications**: Provides tools and insights for experimenting with stock market predictions using sentiment and statistical indicators.
- **Educational Value**: The code and documentation are designed to be accessible and reproducible for readers interested in stock market analysis and machine learning.

---

## Technologies Used
- **Python Libraries**: `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `nltk`, `tensorflow`, `keras`
- **Tools**: Jupyter Notebooks, VADER for sentiment analysis, LSTMs for time-series predictions
- **Data Sources**: Articles scraped from [Financial Post](https://business.financialpost.com) and historical stock price data from Yahoo! Finance

---
