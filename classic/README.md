# Classic Machine Learning Modelling

Any Machine Learning Model be it GPT, BERT or SVM, all require text in a specific format. By specific format I mean it as numbers. Any ML model requires numbers as input. They cannot process text or images as is. We need to create features that the model can understand.

## What is feature engineering?

Feature engineering is handcrafting features to feed into the ML model so that it can understand / process them. We need to convert the raw data it can be images or text to feature vectors (feature vector is just a fancy word for a matrix) since all ML models perform mathematical operations in them and mathematics require numbers.

## Text Feature Engineering

For text feature engineering we have many methods:

* Label Encoding

Bag of words is basically building a collection of list of all words present in the training dataset. 

For example the sentence "Let's build a text classifier" as `[5, 10, 2, 1, 6]` where each word is represented as an index in the vocabulary. This is most simple approach of feature engineering in text. This is similar to label encoding.

* One Hot Encoding

One hot encoding is the same concept as the label encoding but it uses one hot vectors.


The above two approaches are generally not used in practical NLP due to the following disadvantages:
1. These approaches do not capture the meaning of the words.
2. One hot encoding consumes too much memory because for representing one word with a vocabulary size of 100k, we would have a vector length of 100k.
3. OOV (Out of vocabulary) problem. Every new word that we encounter would be represented as OOV which is not accurate.
4. No fixed length representation, since when we flatten the one hot encoding vector (make 4 lists into one), the size can vary.

* Bag of words
* TF-IDF
* Word Embeddings