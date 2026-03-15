# AI Fake Job & Internship Detector

An AI-powered web application that detects whether a job or internship posting is **real or fraudulent** by analyzing the content of the job posting URL using **Machine Learning and Natural Language Processing (NLP)**.

This project was developed as part of research work on detecting fraudulent online job postings.

---

## Research Title

**Detecting Fraudulent Online Job and Internship Postings Using Machine Learning and Natural Language Processing**

---

## Problem Statement

Online job platforms are increasingly targeted by scammers posting fake job and internship opportunities. These postings often ask applicants to pay registration fees, training fees, or deposits.

This system helps identify such scams by analyzing job descriptions and detecting suspicious patterns using machine learning.

---

## Features

* Detects **Fake vs Real job postings**
* Accepts **URL of job posting**
* Scrapes webpage content automatically
* Uses **NLP-based text analysis**
* Provides:

  * Prediction (Real / Fake)
  * Confidence Score
  * Risk Level
  * Suspicious Indicators
* Interactive **AI-powered web interface**
* Research dashboard with model comparison and dataset statistics

---

## Technology Stack

### Backend

* Python
* Flask

### Machine Learning

* scikit-learn
* TF-IDF Vectorization
* Logistic Regression
* Random Forest
* Naive Bayes

### Data Processing

* pandas
* numpy
* nltk

### Web Scraping

* BeautifulSoup
* requests

### Frontend

* HTML
* CSS
* JavaScript
* Bootstrap

---

## Dataset

Dataset used for training:

Fake Job Postings Dataset from Kaggle

https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction

Dataset includes:

* Job Title
* Company Profile
* Job Description
* Requirements
* Benefits
* Fraudulent Label (0 = Real, 1 = Fake)

---

## Machine Learning Pipeline

1. Data Cleaning
2. Text Preprocessing
3. TF-IDF Vectorization
4. Train/Test Split
5. Model Training
6. Model Evaluation
7. Best Model Selection
8. Model Saving using Joblib

Models compared:

* Logistic Regression
* Random Forest
* Naive Bayes

---

## Project Structure

```
fake_job_detector/

app.py
requirements.txt

model/
train_model.py
saved_model.pkl

scraper/
scraper.py

dataset/
fake_job_postings.csv

templates/
index.html
detector.html
about.html
contact.html

static/
css/
js/
images/
```

---

## How to Run the Project

### 1 Install Dependencies

```
pip install -r requirements.txt
```

### 2 Download Dataset

Download the dataset and place it inside the dataset folder:

```
dataset/fake_job_postings.csv
```

### 3 Train the Model

```
python model/train_model.py
```

### 4 Run the Application

```
python app.py
```

### 5 Open the Website

```
http://localhost:5000
```

---

## Example Use Case

User pastes a job posting URL:

```
https://example.com/job-posting
```

System will:

1. Scrape job description
2. Process text using NLP
3. Predict fraud probability
4. Display result

Output example:

Prediction: Fake Job
Confidence: 87%
Risk Level: High

Detected Indicators:

* Registration fee mentioned
* Unrealistic salary
* Suspicious contact information

---

## Research Contributions

This system demonstrates how machine learning and NLP techniques can help detect fraudulent job postings by analyzing linguistic patterns and suspicious indicators.

The platform also provides visualizations such as:

* Model accuracy comparison
* Confusion matrix
* Feature importance
* Dataset statistics

---

## Future Improvements

* Deep Learning models (BERT)
* Browser extension for job platforms
* Real-time scam reporting
* Larger dataset training

---

## Author

Bhavya Bandarupalli
B.Tech CSE Student
KLH University

LinkedIn
https://www.linkedin.com/in/bhavya-bandarupalli-a948bb385/

Email
[bandarupallibhavya30@gmail.com](mailto:bandarupallibhavya30@gmail.com)

---

## License

This project is created for educational and research purposes.
