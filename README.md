# Text_Classification

Text classification is the process of assigning tags or categories to text according to its content.


# Spam Dataset

The SMS Spam Collection is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages, tagged acording being ham (legitimate) or spam.

The files contain one message per line. Each line is composed by two columns: v1 contains the label (ham or spam) and v2 contains the raw text.

I used Bernoulli Naive Bayes classifier for assigning tags(ham or spam) to texts.

# Naive Bayes Classifier

Principle:- A Naive Bayes classifier is a probabilistic machine learning model that’s used for classification task. The crux of the classifier is based on the Bayes theorem.

Bayes theorem: P(y/X)=(P(X/y)*P(y)) / P(X)

Using Bayes theorem, we can find the probability of y happening, given that X has occurred. Here, X is the evidence and y is the hypothesis. The assumption made here is that the predictors/features are independent. That is presence of one particular feature does not affect the other. Hence it is called naive.

If X is mutli featured i.e., X=(x1,x2,......xn) then

P(y/(x1,x2,...xn))=(P(x1/y)P(x2/y)....P(xn/y)P(y)) / (P(x1)P(x2)..........P(xn))

Suppose we have more than one label means y takes more than one values in the case we calculate probability corresponding to each label and compare the probability with each others. The label for which probabilty is maximum that label is assigned to the corresponding datapoint

# Types of Naive Bayes Classifier:

# Multinomial Naive Bayes:
This is mostly used for document classification problem, i.e whether a document belongs to the category of sports, politics, technology etc. The features/predictors used by the classifier are the frequency of the words present in the document.

# Bernoulli Naive Bayes:
This is similar to the multinomial naive bayes but the predictors are boolean variables. The parameters that we use to predict the class variable take up only values yes or no, for example if a word occurs in the text or not.

# Gaussian Naive Bayes:
When the predictors take up a continuous value and are not discrete, we assume that these values are sampled from a gaussian distribution.
