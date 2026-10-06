# Bayesian Probabilistic Classifier using Bernoulli Naive Bayes

## Aim

To model a simple probabilistic classifier for disease diagnosis and perform prediction using the **Bernoulli Naive Bayes** algorithm in Python.

## Description

This practical uses the **Bernoulli Naive Bayes** classifier from the `scikit-learn` library to predict whether a patient has **Flu** or **Cold** based on three binary symptoms.

Each symptom is represented using:

* `1` – Symptom is present
* `0` – Symptom is absent

The classifier learns from a small training dataset and predicts the diagnosis for new patients.

## Software Requirements

* Python 3.x
* Scikit-learn

## Installation

Install the required library using:

```bash
pip install scikit-learn
```

## Input Features

The three features represent symptoms:

| Feature   | Meaning |
| --------- | ------- |
| Feature 1 | Fever   |
| Feature 2 | Cough   |
| Feature 3 | Fatigue |

For example:

```text
[1, 1, 1]
```

means the patient has all three symptoms.

## Training Dataset

The program uses the following training data:

```text
[1, 1, 1] → Flu
[1, 1, 0] → Flu
[1, 0, 1] → Flu
[0, 1, 0] → Cold
[0, 1, 1] → Cold
[0, 0, 0] → Cold
```

The target classes are:

```text
Flu
Cold
```

## Algorithm Used

### Bernoulli Naive Bayes

Bernoulli Naive Bayes is a probabilistic classification algorithm designed for binary features.

It calculates the probability of each possible class based on the observed features and selects the class with the highest probability.

In this practical:

```python
from sklearn.naive_bayes import BernoulliNB
```

is used to create the classifier.

## Program Steps

1. Import `BernoulliNB` from `sklearn.naive_bayes`.
2. Create the training dataset `X`.
3. Create the corresponding diagnosis labels `y`.
4. Create a Bernoulli Naive Bayes model.
5. Train the model using `model.fit(X, y)`.
6. Provide symptoms of a new patient.
7. Predict the patient's diagnosis using `model.predict()`.
8. Calculate the probability of each diagnosis using `model.predict_proba()`.
9. Display the predicted diagnosis and probabilities.
10. Test another patient with different symptoms.

## Prediction 1

The first patient is:

```python
patient = [[1, 1, 1]]
```

This means the patient has:

* Fever
* Cough
* Fatigue

The model predicts:

```text
Predicted diagnosis: Flu
```

The program also displays the probability of both `Cold` and `Flu`.

## Prediction 2

The second patient is:

```python
patient2 = [[0, 1, 0]]
```

This means the patient has only the second symptom.

The model predicts:

```text
Predicted diagnosis: Cold
```

## Expected Output

The output will be similar to:

```text
Predicted diagnosis: Flu
Cold = 0.08
Flu = 0.92
Predicted diagnosis: Cold
```

*The exact probability values may vary slightly depending on the scikit-learn version and model implementation.*

## Advantages

* Simple and easy to implement.
* Fast for small datasets.
* Works well with binary features.
* Provides probability estimates for predictions.
* Requires relatively little training data.

## Limitations

* Assumes that features are conditionally independent.
* The example uses a very small dataset.
* It is intended for demonstration and is not suitable for real medical diagnosis.
* Accuracy depends on the quality and size of the training data.

## Applications

Bernoulli Naive Bayes can be used for:

* Medical diagnosis classification
* Spam detection
* Text classification
* Sentiment analysis
* Document classification
* Binary feature-based prediction

## Result

The Bernoulli Naive Bayes probabilistic classifier was successfully implemented using Python and the **scikit-learn** library. The model successfully predicted the diagnosis of new patients as **Flu** or **Cold** and also calculated the probability of each diagnosis.
