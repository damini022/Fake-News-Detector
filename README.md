Fake News Detection using Machine Learning

This project is a Fake News Detection system built using Machine Learning. It analyzes the text of news articles and classifies them as **REAL** or **FAKE**. The system is trained using a labeled dataset and uses text preprocessing and TF-IDF for feature extraction, followed by logistic regression for classification.



# Files in This Repository

- `Fake_News_Detector.ipynb` – Main Jupyter Notebook containing the entire code.
- `README.md` – Project overview and instructions.



# Dataset

This project uses the Fake and Real News Dataset from Kaggle, which includes:
- `True.csv` – Real news articles from reliable sources.
- `Fake.csv` – Fake or misleading news articles.

 Dataset Link:  
 [https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)



# Technologies Used

- Python
- Pandas & NumPy
- Scikit-learn
- TF-IDF Vectorizer
- Logistic Regression
- Google Colab



# How It Works

1. Data Loading – Reads two CSV files: one for real news and one for fake news.
2. Labeling – Adds a "label" column: `REAL` for real news and `FAKE` for fake news.
3. Preprocessing – Combines both datasets and cleans the text.
4. Feature Extraction – Applies TF-IDF to convert text into numerical vectors.
5. Model Training – Uses Logistic Regression to train on 80% of the data.
6. Model Evaluation – Evaluates performance using accuracy, precision, and recall.
   



# Current Limitations

- The model currently shows **"FAKE" as output for most inputs** due to dataset imbalance or overfitting.
- Input-based prediction via `input()` may not work properly in Google Colab. You can comment that part if needed.
- You must upload the `True.csv` and `Fake.csv` files every time when using in Colab unless hosted elsewhere.



# Future Improvements

- Use a balanced or weighted classifier.
- Deploy the model via Flask or Streamlit.
- Add data visualizations for better insights.
- Use advanced NLP models like BERT or LSTM for improved accuracy.




