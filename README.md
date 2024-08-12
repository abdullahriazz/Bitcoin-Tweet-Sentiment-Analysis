# Bitcoin Tweet Sentiment Analysis

This project performs sentiment analysis on Bitcoin-related tweets using PySpark. It processes a dataset of tweets to classify their sentiment and generate insightful visualizations.

## Table of Contents

- [Project Overview](#project-overview)
- [Setup](#setup)
- [Usage](#usage)
- [Results](#results)
- [Visualizations](#visualizations)

## Project Overview

The goal of this project is to analyze and visualize sentiment trends in tweets about Bitcoin. The pipeline includes:

1. **Data Cleaning:** Remove irrelevant content and preprocess tweets.
2. **Sentiment Analysis:** Apply sentiment analysis to categorize tweets as positive, negative, or neutral.
3. **Model Training and Evaluation:** Train a Logistic Regression model to predict tweet sentiment and evaluate its performance.
4. **Data Visualization:** Generate various visualizations to explore sentiment distribution, keyword frequency, tweet volume over time, and more.

## Setup

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/yourusername/bitcoin-tweet-sentiment-analysis.git
    cd bitcoin-tweet-sentiment-analysis
    ```

2. **Install Dependencies:**

    Ensure you have PySpark and the necessary Python libraries installed. You can install them using `pip`:

    ```bash
    pip install pyspark nltk matplotlib seaborn pandas plotly wordcloud
    ```

3. **Download NLTK Data:**

    The script uses NLTK's Vader lexicon for sentiment analysis. Ensure the data is downloaded:

    ```python
    import nltk
    nltk.download('vader_lexicon')
    ```

4. **Spark Setup:**

    Ensure you have Apache Spark installed and properly configured. This project assumes Spark is set up locally.

5. **Hadoop Setup:**

    Ensure you have Hadoop installed and properly configured. This project assumes Hadoop is set up locally.

## Usage

1. **Prepare Your Data:**

    Place your tweet data in a CSV file at the specified path (`hdfs://localhost:9000/dir/tweets.csv`). The CSV should contain a `text` column with the tweet content.

2. **Run the Analysis:**

    Execute the PySpark Jupyter Notebook to perform the sentiment analysis

## Results

- **Model Performance:**
  - Accuracy: 91.37%
  - Precision: 91.37%
  - Recall: 91.36%
  - F1-score: 91.32%

- **Sentiment Distribution:**
  - Positive: 629 tweets
  - Neutral: 1086 tweets
  - Negative: 285 tweets

## Visualizations

1. **Distribution of Sentiment Scores:**
   ![Distribution of Sentiment Scores](https://github.com/user-attachments/assets/2f8c3cf8-1947-4086-b6c9-6b1f2b13871f)

2. **Word Cloud of Most Frequent Terms:**
   
   ![Word Cloud of Most Frequent Terms](https://github.com/user-attachments/assets/676936de-62b9-4556-957c-748f17ba0c24)

3. **Tweet Volume Over Time:**
   
   ![Tweet Volume Over TIme](https://github.com/user-attachments/assets/36ea5987-4d23-4d81-9a74-749f378cfeb6)


For any questions or feedback, contact me at [abdullahriaz.work@gmail.com]([abdullahriaz.work@gmail.com).
