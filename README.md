# Purpose of the Project:
1. Utilize NLP techniques to manage and analyze textual information.
2. Conduct initial data analysis and generate visual representations in the form of Word Clouds.
3. Use the Natural Language Toolkit (NLTK) for breaking down text into individual elements or tokens.
4. Implement feature extraction by employing a Count Vectorizer method.
5. Comprehend the principles behind the Naive Bayes algorithm, including the distinctions among marginal likelihood, likelihood, and prior probability in statistical terms.
6. Train classifiers based on Naive Bayes and Logistic Regression using the scikit-learn library to predict outcomes from textual datasets. <br />

In retail companies, Natural Language Processing helps build predictive models to perform sentiment analysis based on social media posts/reviews, and assess if customers are satisfied with a product or not. NLP encodes words to numbers and trains a model to make corresponding predictions. As a result, we can easily assess how customers felt about a product without manually checking a large number of reviews.

Generally, NLP can work with input data in image, video, and text formats. In this project, we will perform sentiment analysis on textual data.

We have vast data on product reviews in text format. We would like to predict whether or not customers are satisfied with the product. Our data has the ratings (as in number of starts), the date of review, the variations of the product sold, the verified customer reviews of the product, and the feedback column of values 1 (if ratings are >=4) and 0 (if ratings are <= 2).

# Understanding Tokenization (Count Vectorization):
We want to feed data into an ML classifier. We want to convert our data into a numerical format. To do this, we will apply tokenization.

1. We create a list of columns for every unique word in the strings of the whole column.
2. We will take the strings one after another, and indicate '1' if the word exists in the string, and '0' otherwise (based on the corresponding word column) and populate the word columns accordingly based on its existence in each string. <br />

We will leverage sklearn for feature extraction and count vectorization for us.

# Understanding Logistic Regression Classification:
1. Logistic Regression is a statistical method used for binary classification, which predicts the probability of a data point belonging to one of two possible categories.
2. The technique uses a logistic function to model the probability that a given input belongs to the default class, which can be expressed as a value between 0 and 1. This function estimates the odds of the occurrence of an event by fitting data to a logistic curve.
3. It calculates the relationship between the dependent binary variable and one or more independent variables by estimating probabilities using a logistic function, which is typically a sigmoid curve.
4. The outcome is then transformed into a binary decision using a threshold value, typically 0.5, where probabilities above this threshold are classified as one class, and those below are classified as the other.
5. Logistic Regression is particularly useful for cases where the relationship between the independent variables and the dependent variable is not linear, allowing for more complex relationships to be modeled.

# Understanding Naive Bayes Classification:
1. The Naive Bayes classifier is a predictive modeling technique based on Bayes' Theorem.
2. It involves computing two key components: the prior probability, which is an initial estimate of classifying a data point into a particular category without considering its features, and the likelihood, which is the probability of classifying a data point into a category based on the features of nearby data points.
3. These two elements, the prior probability and likelihood, are integrated to determine the posterior probability according to Bayes' Theorem. A data point is assigned to the class for which it has the highest posterior probability.
4. In essence, the posterior probability is calculated as the product of the likelihood and the class's prior probability, divided by the marginal likelihood.
5. The classification of a data point is ultimately based on which class has the greatest posterior probability.
