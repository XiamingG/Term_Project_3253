# Sentiment Analysis of Chinese Short Texts

This project is for course scs3253 Machine Learning term project

**Ximaing.Gu** caroline3599@gmail.com

2019.08.20


## Abstract

This notebook classifies movie reviews as positive or negative using the text of the comments. I use two modules.

* Naive_bayes Model to Classfire the reviews

* tf.keras, a high-level API to build and train models in TensorFlow. 

## Dataset

### Download the DMSC dataset

Dataset is from https://www.kaggle.com/utmhikari/doubanmovieshortcomments.

Douban Movie is a Chinese website that allows Internet users to share their comments and viewpoints about movies. Users are able to post short or long comments on movies and give them marks. 

### Stopwords 
The library for stop words is from https://github.com/goto456/stopwords Use the "哈工大停用词表.txt"

## Naive_bayes Model to Classfire the reviews

Using Pipeline and 
* CountVectorizer
* MultinomialNB

## Deep Convolutional Neural Networks （CNN）
* Input layer, which defines the length of the input sequence.
* Embedding layer. Define the matrix as vocab_size×64, every trainning batch is maxword×64 <br>
* Convolution layer, with 32 filters, the kernel size defines the number of words to be considered when the convolution is passed in the input text document, thus providing grouping parameters.<br>
* MaxPooling1D layer merge the output of the convolution layer.
* Flatten, transforms the format of the matrix  maxword×64 from a 2d-array , to a 1d-array of maxword×64 vector <br>
* This fixed-length output vector is piped through a fully-connected (Dense) layer with (2000, 500, 200, 50, 16) hidden units.  <br>
* The last layer is densely connected with a single output node. Using the sigmoid activation function, this value is a float between 0 and 1, representing a probability, or confidence level..<br>
* Loss function and optimizer<br>

