# NLP-to-Understand-Side-effects-of-melatonin


## Overview
This project is centered around a real-world dataset that requires careful cleaning and organization. The focus is on extracting meaningful insights from product reviews, including sentiment analysis and text analytics, followed by the application of machine learning techniques for classification tasks.

## Project Steps

### 1. Data Preparation and Cleaning
- **Objective:** Organize and merge various CSV files into a single dataframe.
  - **Tasks:**
    - Remove unnecessary features.
    - Extract 'dose' information from the "product_title" column and add it as a new column in the dataframe.

### 2. Sentiment Analysis on Review Ratings
- **Objective:** Perform sentiment analysis based on the "review_rating" column.
  - **Focus:** Analyze sentiments for each dose, not brand.
  - **Tools Used:** NLTK's Sentiment Intensity Analyzer for assessing sentiment.

### 3. Text Analysis on Review Text
- **Objective:** Analyze the "review_text" column.
  - **Tasks:**
    - Remove high-frequency, non-informative words (e.g., 'I', 'the', 'is').
    - Identify and analyze key phrases or words indicating product efficacy or issues (e.g., 'good sleep', 'dissolve', 'tasty', 'helpful', 'no help').
    - Use text analysis tools (e.g., TF-IDF, NLTK) to evaluate reactions and evaluations based on different doses (e.g., 1mg, 2mg, 5mg, 10mg, 25mg).
  - **NLTK Libraries Used:**
    - `nltk`: For natural language processing tasks.
    - `pos_tag` and `word_tokenize`: For tokenizing and tagging words in the review text.
    - `wordnet`: For lemmatization and understanding word meanings.
    - `SentimentIntensityAnalyzer`: For evaluating the sentiment of review texts.

### 4. Machine Learning Models for Dose Prediction
- **Objective:** Train and test machine learning models to predict the choice of doses based on the analysis.
  - **Tasks:**
    - Split the data into training and test sets.
    - Train two different classification models.
    - Evaluate the accuracy and effectiveness of these models in predicting the appropriate dose based on analyzed factors.


## Conclusion
This project aims to demonstrate the ability to handle real-world data, apply sentiment and text analysis techniques, and leverage machine learning for predictive modeling. The key is to derive actionable insights that can inform decision-making processes.
