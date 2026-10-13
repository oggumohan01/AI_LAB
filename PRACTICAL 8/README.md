# PRACTICAL 8

## Title

Development of a Mini AI Application: Text Classification using Python.

## Aim

To develop a mini AI application that classifies text messages as Spam or Not Spam using machine learning.

## Objectives

* To understand text classification in Artificial Intelligence.
* To implement a Naive Bayes classification algorithm.
* To train an AI model using sample text messages.
* To predict whether a message is spam or not spam.
* To understand ethical and explainability considerations in AI.

## Requirements

* Python 3.x
* Scikit-learn library

## Installation

Install the required library using the following command:

```bash
pip install scikit-learn
```

## Theory

Text classification is a Natural Language Processing (NLP) technique that categorizes text into predefined classes.

This application uses a **Naive Bayes classifier** to classify messages into two categories: Spam and Not Spam.

The program uses the following components:

* **CountVectorizer:** Converts text messages into numerical word-count features.
* **MultinomialNB:** Implements the Naive Bayes algorithm for classification.
* **Pipeline:** Combines text vectorization and classification into a single workflow.

The model learns from labelled sample messages and predicts the category of new messages.

## Algorithm

1. Import the required libraries.
2. Create a dataset containing sample messages.
3. Assign Spam or Not Spam labels to the messages.
4. Create a machine-learning pipeline using CountVectorizer and MultinomialNB.
5. Train the model using the dataset.
6. Prepare test messages.
7. Predict the category of each test message.
8. Display the messages and their predicted categories.

## Procedure

1. Write the Python program and save it as `practical8.py`.
2. Install Scikit-learn.
3. Execute the program.
4. Observe the predicted categories displayed on the screen.

## Expected Output

```text
AI TEXT CLASSIFICATION - SPAM DETECTION
---------------------------------------
Message: You won a free gift
Prediction: Spam

Message: Please attend the meeting today
Prediction: Not Spam

Message: Claim your cash prize now
Prediction: Spam
```

## Ethics Considerations

1. **Privacy:** Personal messages should not be used for training without appropriate permission.
2. **Bias:** A small or unbalanced dataset may produce unfair or inaccurate predictions.
3. **Accuracy:** The model may incorrectly classify legitimate messages as spam.
4. **Human Oversight:** Important messages should not be automatically deleted based only on AI predictions.
5. **Transparency:** Users should know when AI is being used to classify messages.
6. **Responsible Use:** The system should be tested before being used in real-world applications.

## Explainability Considerations

* CountVectorizer converts messages into word-count features that can be inspected.
* Naive Bayes uses learned word patterns to estimate the probability of each category.
* The model's predictions depend on the examples used during training.
* The system does not provide a detailed explanation for every individual prediction.
* A larger dataset and suitable evaluation methods can improve reliability and understanding.

## Limitations

* The application uses a small training dataset.
* It may not understand sarcasm, context, or unfamiliar words.
* Predictions may be inaccurate for real-world messages.
* The application is intended for educational purposes, not as a production-ready spam filter.

## Result

The mini AI text-classification application was successfully implemented using Python and the Naive Bayes algorithm. The application classifies sample text messages as Spam or Not Spam and highlights important ethical and explainability considerations in AI.
