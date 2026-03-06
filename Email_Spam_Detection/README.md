# Email Spam Detection using Machine Learning

## Overview
This project builds a **Machine Learning model to detect spam emails**. Spam messages are unwanted emails that are often used for advertisements, scams, or phishing attacks. Using machine learning techniques, the model analyzes the text content of emails and classifies them as **Spam** or **Ham (Not Spam)**.

The project uses **Natural Language Processing (NLP)** techniques to convert email text into numerical features and then trains a classification model to identify spam messages.

## Objective
The main objective of this project is to:
* Analyze email message data
* Preprocess text data for machine learning
* Train a machine learning model for spam detection
* Classify emails as **Spam or Not Spam**

## Dataset
The dataset used in this project contains SMS/email messages labeled as spam or ham.

### Dataset Features
| Column  | Description                                  |
| ------- | -------------------------------------------- |
| label   | Indicates whether the message is spam or ham |
| message | The content of the email/SMS message         |

Example data:
| label | message                               |
| ----- | ------------------------------------- |
| ham   | Go until jurong point, crazy...       |
| spam  | Free entry in a weekly competition... |

## Technologies Used
The project is implemented using the following tools and libraries:
* **Python**
* **Pandas** – Data handling and preprocessing
* **NumPy** – Numerical operations
* **Scikit-learn** – Machine learning models
* **Matplotlib & Seaborn** – Data visualization
* **TF-IDF Vectorizer** – Text feature extraction

## Project Workflow
### 1. Data Loading
The dataset is loaded using the Pandas library.

### 2. Data Preprocessing
* Removed unnecessary columns
* Renamed columns for clarity
* Converted labels from text to numerical values

### 3. Text Vectorization
The email text is converted into numerical form using **TF-IDF (Term Frequency-Inverse Document Frequency)**.
This technique measures the importance of words in messages.

### 4. Train-Test Split
The dataset is split into training and testing sets:
* **80% training data**
* **20% testing data**

### 5. Model Training
A **Multinomial Naive Bayes classifier** is used to train the spam detection model.
This algorithm is widely used for text classification tasks.

### 6. Model Evaluation
The performance of the model is evaluated using **Accuracy Score** and classification metrics.

## Model Performance
The model achieves an accuracy of approximately **97% – 99%** on the testing dataset, indicating high effectiveness in detecting spam messages.

## Project Structure
Email_Spam_Detection
├── data
│   └── spam.csv
├── email_spam_detection.ipynb
├── spam_model.pkl
└── README.md

## How to Run the Project
### 1. Clone the repository
git clone https://github.com/your-username/OIBSIP2.git

### 2. Navigate to the project folder
cd Email_Spam_Detection
### 3. Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn
### 4. Run the notebook
Open and run:
email_spam_detection.ipynb

## Example Prediction
Example input message:
Congratulations! You have won a free prize.

Model prediction:
Spam Message

## Learning Outcomes
Through this project, the following concepts were implemented:
* Natural Language Processing basics
* Text vectorization using TF-IDF
* Machine learning classification
* Model evaluation techniques
