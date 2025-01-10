This project focuses on performing sentiment analysis on a  dataset with 1.6 million tweets using machine learning technique. The dataset, contains labeled tweets indicating whether the sentiment is positive or negative. The goal is to process the text data, clean it, and train a machine learning model to classify tweets into these two sentiment categories.

**Data Cleaning and Preprocessing**

_Renaming Columns:_ The dataset columns are renamed for clarity
_Sentiment Labeling: _The original sentiment labels (0 for negative, 4 for positive) are replaced with binary values—0 for negative and 1 for positive.

**Text Preprocessing**

_Stopword Removal: _Common stopwords such as "the," "is," "in," etc., which do not contribute significant meaning to sentiment analysis, are removed using the NLTK library.

_Stemming:_ The Porter Stemmer is applied to reduce words to their root form .

_Regular Expressions:_ Non-alphabetical characters and numbers are removed from the text to maintain only meaningful words for sentiment analysis.

**Text Representation**

_Vectorization:_ The TfidfVectorizer from Scikit-learn is used to convert the text data into numeric form , which is required for machine learning models to interpret the data.

**Model Training**

_Splitting the Data:_ The dataset is split into training and testing subsets using train_test_split from Scikit-learn.

_Logistic Regression:_ A Logistic Regression model is chosen due to its efficiency and simplicity in binary classification tasks like sentiment analysis.

**Model Evaluation**

_Accuracy Score:_ After training the model, the accuracy score is calculated to evaluate how well the model performs on the test set.
