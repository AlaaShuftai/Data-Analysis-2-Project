# Data-Analysis-2-Project
# Market Basket Analysis and Text Analysis

## Overview
This project involves two primary analyses: Market Basket Analysis and Text Analysis. It aims to extract insights from consumer behavior in retail transactions and customer sentiments from reviews. The datasets utilized for these analyses are sourced from Kaggle:

- **Yelp Dataset**: [Yelp Dataset](https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset)
- **E-commerce Data**: [E-commerce Dataset](https://www.kaggle.com/carrie1/ecommerce-data)

## Table of Contents
- [Technologies Used](#technologies-used)
- [Datasets](#datasets)
- [Market Basket Analysis](#market-basket-analysis)
- [Text Analysis](#text-analysis)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- NLTK
- Plotly

## Datasets
1. **Yelp Dataset**:
   - Contains user reviews and tips for various businesses.
   - Provides insights into customer sentiments and behaviors.
   - Used for performing sentiment analysis.

2. **E-commerce Data**:
   - Includes transaction data from an online retailer.
   - Used for conducting Market Basket Analysis to identify frequently bought items together.

## Market Basket Analysis
### Objective
The goal of Market Basket Analysis is to understand consumer purchasing patterns by identifying associations between different items in transactions.

### Methodology
- **Data Preprocessing**: Cleaning and preparing transaction data for analysis.
- **Association Rule Mining**: Implementing the Apriori algorithm to find frequent itemsets and generate association rules.
- **Visualization**: Using plots to showcase the relationships between products.

### Insights
- Key insights about customer purchasing patterns.
- Recommendations for product placements and promotions based on the analysis.

## Text Analysis
### Objective
The aim of Text Analysis is to analyze customer reviews to gauge sentiment and extract meaningful insights about customer experiences and preferences.

### Methodology
- **Data Preprocessing**: Cleaning and tokenizing text data, removing stopwords, and performing sentiment analysis.
- **Model Training**: Using machine learning models like Naive Bayes to classify sentiments of reviews.
- **Visualization**: Creating plots to visualize common words and sentiment distribution.

### Insights
- Understanding customer sentiments towards products.
- Identifying common themes and areas for improvement based on customer feedback.

## Installation
To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/market-basket-analysis-text-analysis.git
   cd market-basket-analysis-text-analysis
