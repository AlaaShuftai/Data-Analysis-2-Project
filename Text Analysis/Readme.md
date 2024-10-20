## Text Analysis (Extra Model)

### 1. Data Loading and Preprocessing
The analysis starts by loading Yelp's dataset files, which contain user tips and check-ins. The text data from these files is processed for further analysis.

#### Text Processing:
A custom function `text_process` is defined to handle the preprocessing of text data. The steps include:
- **Removal of punctuation**: To clean the text by excluding irrelevant symbols.
- **Tokenization**: Splitting the text into individual words or tokens.
- **Stopword filtering**: Removing common words (like "the", "is", "at") that don't carry much meaning in sentiment analysis.

This preprocessing step improves the quality of the data for the machine learning model.

### 2. Data Transformation
To enhance the text data for analysis:
- The `compliment_count` feature is categorized into star ratings using the `pd.cut()` function.
- The text data is processed through the `text_process` function and stored in a new column named `processed_text`.

### 3. Text Analysis
A frequency count of words is conducted to uncover the most common terms used in user tips:
- **Word Frequency Analysis**: Using `Counter` from the `collections` module, the most frequent words in user reviews are identified.
- **Visualization**: A bar plot is created to visually represent word frequencies, highlighting key phrases users often mention in their reviews.

### 4. Model Training and Evaluation
The preprocessed text data is used to train a machine learning model:
- **Data Splitting**: The dataset is split into training (80%) and testing (20%) sets using `train_test_split`.
- **Vectorization**: The text is converted into numerical data through `CountVectorizer`, which transforms the text into a vectorized format.
- **Model Training**: A Complement Naive Bayes model is trained on the vectorized data.
- **Evaluation**: Predictions are made on the test set, and the model's performance is evaluated using:
  - **Accuracy score**.
  - A **classification report** that provides precision, recall, and F1-score for each star rating (class).

### 5. Performance Metrics
After training the model, the following metrics are computed to assess its performance:
- **Accuracy**: The overall accuracy of the model on the test data is printed.
- **Classification Report**: Precision, recall, and F1-score for each star rating class are provided, revealing how well the model performed across different ratings.

### 6. Additional Data Analysis
Further analysis is performed on other aspects of the dataset:
- **Business ID Length Analysis**: A histogram of the lengths of the `business_id` column is generated to provide insights into the distribution of business ID lengths.
- **Frequency Analysis of `business_id`**: Similar to the word frequency analysis, the frequency of business IDs is calculated and visualized in a bar plot.

### Summary Report

#### Text Preprocessing
- **Methods Used**:
  - Removal of punctuation and stopwords.
  - Tokenization to break text into meaningful units.
- **Impact**: These preprocessing steps helped reduce noise and enhance the model's ability to interpret meaningful patterns in the data.

#### Model Performance
- **Model Used**: Complement Naive Bayes.
- **Accuracy**: The model achieved an accuracy of approximately `X%` (replace with actual accuracy from results).
- **Classification Report**: The classification report provides insights into how well each star rating category was predicted. It highlights categories that were easier to classify and those that were more frequently misclassified.

#### Insights from Analysis
- **Word Frequency**: The most common words in user reviews offer valuable insights into customer sentiments, recurring themes, and areas of concern.
- **Star Rating Distribution**: Understanding the distribution of ratings provides businesses with actionable insights into customer satisfaction levels.

### Conclusion
This analysis demonstrates how sentiment analysis on Yelp data can be performed using a Naive Bayes classification model. The combination of text preprocessing, model evaluation, and data visualization creates a strong framework for text classification tasks. The results can help businesses better understand customer feedback and identify areas for improvement, ultimately leading to enhanced customer satisfaction.
