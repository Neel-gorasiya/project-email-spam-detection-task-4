# Email Spam Detection Using Machine Learning

## Project Overview

Email Spam Detection is a Machine Learning project that classifies emails as **Spam** or **Ham (Not Spam)**. Spam emails often contain advertisements, scams, phishing links, or unwanted content. This project uses Natural Language Processing (NLP) and Machine Learning techniques to automatically identify and filter such emails.

The model is trained on a labeled dataset of emails and learns patterns that help distinguish spam emails from legitimate ones.

---

## Objectives

* Detect whether an email is Spam or Ham.
* Apply text preprocessing and feature extraction techniques.
* Train a Machine Learning model for email classification.
* Evaluate model performance using standard metrics.
* Provide predictions for new email messages.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook / VS Code

---

## Machine Learning Workflow

1. Load the dataset.
2. Clean and preprocess the data.
3. Convert email text into numerical features using TF-IDF.
4. Split the dataset into training and testing sets.
5. Train the Machine Learning model.
6. Evaluate model performance.
7. Predict whether a new email is Spam or Ham.

---

## Dataset

The dataset contains two main columns:

| Column   | Description            |
| -------- | ---------------------- |
| Category | Spam or Ham label      |
| Message  | Email/SMS text content |

Example:

| Category | Message                                |
| -------- | -------------------------------------- |
| ham      | Hi, how are you?                       |
| spam     | Congratulations! You won a free prize. |

---

## Model Used

### Multinomial Naive Bayes

Multinomial Naive Bayes is widely used for text classification tasks because:

* It is simple and fast.
* It performs well on text data.
* It requires less computational power.
* It provides high accuracy for spam detection.

---

## Feature Extraction

The project uses **TF-IDF (Term Frequency-Inverse Document Frequency)** to convert text messages into numerical vectors that can be processed by Machine Learning algorithms.

TF-IDF helps identify important words while reducing the impact of common words.

---

## Evaluation Metrics

The model is evaluated using:

* Accuracy Score
* Confusion Matrix
* Precision
* Recall
* F1-Score

---

## Project Structure

```text
Email-Spam-Detection/
│
├── spam.csv
├── Email_Spam_Detection.ipynb
├── README.md
├── requirements.txt
└── screenshots/
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/email-spam-detection.git
```

Move to the project directory:

```bash
cd email-spam-detection
```

Install required libraries:

```bash
pip install -r requirements.txt
```

---

## Required Libraries

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## Running the Project

Run the Jupyter Notebook:

```bash
jupyter notebook
```

or execute the Python script:

```bash
python spam_detection.py
```

---

## Sample Prediction

Input Email:

```text
Congratulations! You have won a free iPhone. Click here to claim your reward.
```

Output:

```text
Spam
```

Input Email:

```text
Hello, your meeting is scheduled for tomorrow at 10 AM.
```

Output:

```text
Ham (Not Spam)
```

---

## Results

The trained model achieves high accuracy in classifying spam and legitimate emails. The exact accuracy may vary depending on the dataset and preprocessing steps used.

---

## Future Improvements

* Deploy the model as a web application using Flask or Streamlit.
* Add support for real-time email filtering.
* Use advanced NLP techniques.
* Compare multiple Machine Learning algorithms.
* Integrate phishing email detection.

---

## Learning Outcomes

Through this project, the following concepts were explored:

* Data Preprocessing
* Natural Language Processing (NLP)
* Feature Extraction using TF-IDF
* Machine Learning Classification
* Model Evaluation
* Data Visualization

---

## Conclusion

This project demonstrates how Machine Learning can be used to automatically detect spam emails. By combining TF-IDF feature extraction with the Multinomial Naive Bayes algorithm, the system can effectively classify emails and help users avoid unwanted or potentially harmful messages.
