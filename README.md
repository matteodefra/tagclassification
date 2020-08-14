# Tag Classification
My final project for Bachelor's thesis, an implementation of a neural network for category classification of popular site StackOverflow
## Introduction
I studied the problem of category classification on [StackOverflow](https://stackoverflow.com/). After a preliminary analysis on the data and the different categories categories and distributions, I ended up creating a C-LSTM neural network.
## The work
I mixed two convolutional neural network followed by a long-short term memory network. For first I cleaned the text of questions, tokenized it and for last transformed in sequences. I gave these sequences to the convolutional neural network to select best features and after the selected features are given to the LSTM for text classification. I ended up doing a training phase and testing phase selecting the top 8 categories predicted, having a range of possibilities. 
## Results
Using this strategy I obtained the following results:
1. First Tag, with 1223 distinct values, testing accuracy = 83%
1. Second Tag, with 4304 distinct values, testing accuracy = 47%
1. Third Tag, with 10886 distinct values, testing accuracy = 23%
## Improvements
Restricting the number of values for each Tags will give a better accuracy but on a subset of data, I decided to use all the possible values in this study.
Using techniques like NLP toolkit or bag of words method gave the same results.
