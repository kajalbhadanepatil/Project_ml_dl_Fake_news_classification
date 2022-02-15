# Project_ml_dl_Fake_news_classification
## Overview
* **Motivation:**
The topic of fake news is as old as the news industry itself — misinformation, hoaxes, propaganda, and satire have long been in existence. 
Fake news undermines serious media coverage and makes it more difficult for journalists to cover significant news stories.
The reasons behind fake news include media manipulation and propaganda, political and social influence, provocation ans social unrest and financial profit 
* **Problem Statement:**
Classify news as fake or real using various ML and DL algorithms

## Working Methodology 
* EDA 
  * Check null
  * CHeck class distribution 
  * Analyse the No of characters present in title and text according to label
  * N-gram analysis
  * Word cloud
* Preprocessing of data
  * Get the Dependent feature
  * Reset Index of our Dataset
  * Data cleaning
      * Step 1 -- re.sub -- Consider only alphabets and removing the numbers, special characters
      * Step 2 -- review.lower() -- Converting all the words to lower case
      * Step 3 -- review.split() -- Convert the whole text into a list of words, so that the stop words can be applied to them later
      * Step 4 -- ps.stem() -- Stemming-Is the process of producing morphological variants of a root/base word. A stemming algorithm reduces the words “chocolates”, “chocolatey”, “choco” to the root word, “chocolate”
      * Step 5 -- stopwords.words('english') -- Removing stopwords Stopwords - Words like a, the , is , then etc are redundant and doesn't play any role in nlp, so it's better to remove these type of words. And stop words is the way to do that.
      * Step 6 -- ' '.join() -- joining them again
  * One-hot Encoding
  * Text Padding
  * Train test split
* Model building - I used two inputs for building the model 
  * Title 
      * Naive bayes
      * Linear SVM 
      * KNN
      * LSTM Model 
      * LSTM model using dropout layer 
      * LSTM model using CNN layer
  * Text 
      * LSTM Model 
      * LSTM model using dropout layer 
## Data collection 
I used the dataset from Kaggle 

## Technical Aspect 
* Python -- Programming Langauge for this Notebook.
* Pandas -- Python Data Analysis Library.
* Sklearn -- Machine Learning handling in Python.
* Matplotlib -- creating static, animated, and interactive visualizations in Python.
* Seaborn -- Python data Visulization based on matplotlib.
* Rerular Expression -- For data cleaning 
* NLTK -- Used for NLP 
* Wordcloud -- Data visualisation for text data
* Keras -- Python interface for artificial neural networks 
* Tensorflow -- Python library for fast numerical computing 

## Model evaluation criteria 
Accuracy score 

## Results 
|Input |Model|Accuracy_Score|
|:--:|:--:|:--:|
|Title|Naïve bayes| 68.08 %|
|Title|Linear SVM| 70.47 % |
|Title|KNN | 78.04 % |
|Title|LSTM | 89.87 % |
|Title|LSTM with dropout layer | 90.66 % |
|Title|LSTM with CNN layer| 89.85 % |
|Text|LSTM| 91.05 % |
|Text|LSTM with dropout layer | 91.75 % |

## Conclusion 
LSTM model with dropout layer build using text as input gives best results 

  
 

