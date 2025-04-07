# Fake News Predictor

This project implements a Logistic Regression model to classify news articles as either "fake" or "real." The model uses Natural Language Processing (NLP) techniques to preprocess the data and extract meaningful features for classification.

## Features

- **Data Preprocessing**: 
  - Handles missing values by replacing them with empty strings.
  - Merges the `author` and `title` columns into a single `content` column.
  - Applies stemming to reduce words to their root forms.
  - Removes stopwords to focus on meaningful words.

- **Feature Extraction**:
  - Converts text data into numerical feature vectors using `TfidfVectorizer`.

- **Model Training**:
  - Splits the dataset into training and testing sets.
  - Trains a Logistic Regression model on the training data.

- **Evaluation**:
  - Calculates accuracy on both training and testing datasets.
  - Predicts whether a given news article is "fake" or "real."


## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Fake_news_predictor.git
   cd Fake_news_predictor
2. Install the required Python libraries:
   ```bash
   pip install numpy pandas scikit-learn nltk
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Logistic_Regression_Model.ipynb
4. Run the cells in the notebook to:

   - Preprocess the data.
   - Train the Logistic Regression model.
   - Evaluate the model's performance.
5. Test the model with your own news data:
   Modify the news variable in the prediction cell to input your own text.
   Run the prediction cell to classify the news as "fake" or "real."
## Dataset
The dataset (train.csv) contains the following columns:

  - id: Unique identifier for each news article.
  - title: Title of the news article.
  - author: Author of the news article.
  - text: Full text of the news article.
  - label: Target label (1 for fake news, 0 for real news).

## Results
Training Data Accuracy: ~98.66%
Testing Data Accuracy: ~97.91%

  
