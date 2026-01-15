# About the Fake vs Real News Analysis

**Authors**: Federica Gianoglio, Nanditha Lekshmy, Esha More

**GitHub**: https://github.com/federica-gianoglio/fake-vs-real-news-analysis/

**Description**: Descriptive, diagnostic, and predictive analysis of fake vs real news articles. 

## **Project Overview**
This project analyzes a large dataset of real and fake news articles to uncover textual patterns, perform sentiment analysis, and build predictive classifiers.

This program examines fake and real news articles with descriptive, diagnostic, and predictive analysis, culminating in the evaluation of three predictive machine learning models to classify articles as 'fake' or 'real'. 

The three authors contributed to this analysis in equal proportions. Each code cell indicates the contributing author by their first name.

Below are listed the key tasks performed in this program, excluding the data visuals present throughout the entire project. 

**Data Cleaning and Preparation**
* NaN removal
* Column labeling
* Tokenization
* Removal of non-alphabetical characters and stop words
* Stemming

**Descriptive Analysis**
* Calculation of average, median, standard deviation, and mode values
* Skew and kurtosis analyses
* Frequency distribution plots of the top 30 words and word clouds for the top 100 words

**Diagnostic Analysis**
* Correlation analysis
* Sentiment analysis and polarity scores
* Multiple linear regression

**Predictive Analysis**

Three machine learning models were trained and tested using both text and numerical features to identify the best classifier for fake vs real articles:
* Support Vector Machine (SVM)
* Naive Bayes
* Logistic Regression

## **About the Data**
* **Data**: A dataset containing 79k articles divided in two files:
  * MisinfoSuperset_TRUE.csv (34,975 articles with real news)
  * MisinfoSuperset_FAKE.csv (43,642 articles of misinformation, fake news or propaganda)
* **Source**: Two data files are available on Kaggle:
https://www.kaggle.com/datasets/stevenpeutz/misinformation-fake-news-text-dataset-79k/data.
* **Note**: To run the program, load both files to your terminal.

## **Columns**
* ID – Unique article identifier
* text – Content of the article

## **Dependencies**
This project was developed using Python 3.x. The following packages are required to run all analyses and visualizations:

* pandas – data manipulation and analysis
* numpy – numerical computations
* matplotlib – plotting and visualization
* seaborn – statistical visualization
* nltk – natural language processing (requires downloading corpora: punkt, stopwords, averaged_perceptron_tagger, vader_lexicon)
* swifter – faster apply operations on pandas DataFrames
* wordcloud – generate word clouds
* scikit-learn – machine learning models, preprocessing, and metrics
* scipy – sparse matrices and statistical functions
* statsmodels – statistical modeling

**Note**: After installing NLTK (pip install nltk), the required corpora can be downloaded by running:

```
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('averaged_perceptron_tagger')
nltk.download('vader_lexicon')
```
