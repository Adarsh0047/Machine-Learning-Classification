# Classic Machine Learning Modelling

Any Machine Learning Model be it GPT, BERT or SVM, all require text in a specific format. By specific format I mean it as numbers. Any ML model requires numbers as input. They cannot process text or images as is. We need to create features that the model can understand.

## What is feature engineering?

Feature engineering is handcrafting features to feed into the ML model so that it can understand / process them. We need to convert the raw data it can be images or text to feature vectors (feature vector is just a fancy word for a matrix) since all ML models perform mathematical operations in them and mathematics require numbers.

## Text Feature Engineering

For text feature engineering we have many methods:

* Bag of Words
* One hot encoding
* TF-IDF
* Word Embeddings