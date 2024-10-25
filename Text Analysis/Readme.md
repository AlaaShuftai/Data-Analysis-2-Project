## Text Analysis (Extra Model)

### Short description:

In this Task, we performed text analysis to extract insights from textual data. We began with preprocessing steps, including tokenization, converting text to lowercase, and removing punctuation. We then applied TF-IDF to convert text into numerical features for analysis. For visualization, we generated a word cloud to highlight common terms. Finally, we implemented sentiment analysis using Scikit-Learn to understand sentiment trends and patterns in the text data.

### Data
The analysis starts by loading Yelp's dataset files, which contain user tips and check-ins. The text data from these files is processed for further analysis.
Yelp Reviews Dataset (https://www.kaggle.com/yelp-dataset/yelp-dataset)

#### Text Processing:
A custom function `text_process` is defined to handle the preprocessing of text data. The steps include:
- **Removal of punctuation**: To clean the text by excluding irrelevant symbols.
- **Tokenization**: Splitting the text into individual words or tokens.
- **Stopword filtering**: Removing common words (like "the", "is", "at") that don't carry much meaning in sentiment analysis.

This preprocessing step improves the quality of the data for the machine learning model.



- ### libraries we used:
1. kagglehub: A library that helps you interact with Kaggle's datasets.
2. numpy: Short for Numerical Python, it's crucial for array and matrix operations.
3. pandas: Essential for data manipulation and analysis, it uses dataframes.
4. seaborn: A statistical data visualization library based on Matplotlib, making plots more attractive and easier to understand.
5. matplotlib.pyplot: Used for creating static, animated, and interactive visualizations in Python.
6. tensorflow: An open-source platform for machine learning, especially for neural networks.
7. tensorflow.keras.preprocessing.text.Tokenizer: A tool for tokenizing text data for deep learning models.
8. sklearn.metrics: Various modules for evaluating the performance of machine learning models.
9. sklearn.svm.LinearSVC: A Linear Support Vector Classification model.
10. sklearn.feature_extraction.text.TfidfVectorizer: Converts a collection of raw documents to a matrix of TF-IDF features.
11. sklearn.naive_bayes.MultinomialNB: A Naive Bayes classifier for multinomially distributed data.
12. sklearn.model_selection: Tools for splitting datasets and cross-validation.
13. datetime: For manipulating dates and times.
14. string: Common string operations.
15. nltk: The Natural Language Toolkit, essential for working with human language data.
16. nltk.corpus.stopwords: A collection of stopwords to be filtered out of text data.
17. sklearn.naive_bayes.ComplementNB: A variant of the Naive Bayes classifier.
18. sklearn.feature_extraction.text.CountVectorizer: Converts text documents to a matrix of token counts.
    
### Summary

#### Text Preprocessing
- **Methods Used**:
  - Removal of punctuation and stopwords.
  - Tokenization to break text into meaningful units.
- **Impact**: These preprocessing steps helped reduce noise and enhance the model's ability to interpret meaningful patterns in the data.

- 
#### Insights from Analysis
- **Word Frequency**: The most common words in user reviews offer valuable insights into customer sentiments, recurring themes, and areas of concern.
- **Star Rating Distribution**: Understanding the distribution of ratings provides businesses with actionable insights into customer satisfaction levels.

### Conclusion
This analysis demonstrates how sentiment analysis on Yelp data can be performed using a Naive Bayes classification model. The combination of text preprocessing, model evaluation, and data visualization creates a strong framework for text classification tasks. The results can help businesses better understand customer feedback and identify areas for improvement, ultimately leading to enhanced customer satisfaction.
