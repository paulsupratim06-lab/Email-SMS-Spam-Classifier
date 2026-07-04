# Email & SMS Spam Classifier

A machine learning-powered web application that classifies **Email** and **SMS** messages as **Spam** or **Not Spam (Ham)** using Natural Language Processing (NLP) techniques. The application is built with Python, Scikit-learn, and Streamlit, providing an intuitive interface for real-time spam detection.

---

## Features

- Detects whether an Email or SMS is Spam or Ham
- Text preprocessing using NLTK
- TF-IDF feature extraction
- Includes an additional handcrafted feature:
  - Number of characters in the message
- Interactive web interface built with Streamlit
- Fast and lightweight prediction

---

## Tech Stack

- Python
- Streamlit
- Scikit-learn
- Pandas
- NumPy
- NLTK
- Pickle

---

## Project Structure

```text
Email-SMS-Spam-Classifier/
│
├── main.py                 # Streamlit application
├── model.pkl               # Trained machine learning model
├── vectorizer.pkl          # TF-IDF Vectorizer
├── requirements.txt
├── spam.csv                # Dataset
├── README.md
└── ...
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/paulsupratim06-lab/Email-SMS-Spam-Classifier.git
```

Navigate to the project directory:

```bash
cd Email-SMS-Spam-Classifier
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Download the required NLTK resources:

```python
import nltk

nltk.download('punkt')
nltk.download('stopwords')
```

---

## Running the Application

Start the Streamlit application:

```bash
streamlit run main.py
```

The application will open automatically in your default web browser.

---

## Workflow

1. The user enters an Email or SMS message.
2. The text is preprocessed.
3. Stopwords and punctuation are removed.
4. The remaining words are stemmed.
5. TF-IDF converts the processed text into numerical features.
6. The character count feature is appended.
7. The trained machine learning model predicts whether the message is Spam or Ham.

---

## Machine Learning Pipeline

### Data Preprocessing

- Convert text to lowercase
- Tokenization
- Remove punctuation
- Remove stopwords
- Apply stemming using Porter Stemmer

### Feature Engineering

- TF-IDF Vectorization
- Character count feature

### Prediction

The processed features are passed to the trained classifier, which predicts whether the message is:

- Spam
- Ham (Not Spam)

---

## Dataset

This project uses the SMS Spam Collection Dataset, which contains thousands of labeled SMS messages categorized as Spam or Ham.

---

## Future Improvements

- Email-specific preprocessing
- Prediction confidence score
- Drag-and-drop email (.eml) support
- Spam category classification
- Deep learning models such as LSTM or BERT
- Cloud deployment

---

## Contributing

Contributions are welcome.

To contribute:

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Open a Pull Request.

---

## License

This project is intended for educational and learning purposes.

---

## Author

**Supratim Paul**

GitHub: https://github.com/paulsupratim06-lab
