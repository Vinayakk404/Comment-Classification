# Toxic-Comment-Classification
Done as part of my college coursework

## Overview
This model uses a hybrid of bidirectional LSTM and convolutions to give a neural network structure which uses proprietary lexicons to achieve a structured and labelled
classification of our presented dataset from Kaggle Challenge into different ones like toxic, severely toxic, etc.This model also uses several pre-processing techniques
like parsing, stemming, and removal of punctuations. after that, we use  bidirectional layers including the dense, dropout and a sequential model while splitting our dataset into train(0.7), validation(0.2), and test(0.1).The last step is the prediction stage which helps us predict the results and classify them into labels using a range format.

## Introduction
Online forums and social media platforms have provided Individuals with the means to put forward their thoughts and freely express their opinion on various issues and incidents. In some cases, these online comments contain explicit language which may hurt the readers. Comments containing explicit language can be classified into categories such as Toxic, Severe Toxic, Obscene, Threat, Insult, and Identity Hate. The threat of abuse and harassment means that many people stop expressing
themselves and give up on seeking different opinions.

## Meathodology
After loading the data in our Jupyter notebook we will first

Implement pre-processing

➔Checking for missing values.
First and foremost we will be using the “isnull” function on both the training and test data in order to check if there are any null values present or not. If yes we would filter them out as we do not want to deal with incomplete data

➔Text Normalization.
So the things we will perform are Removing Characters in between Text,Removing Repeated Characters, Converting data to lower-case, Removing Punctuation, unnecessary
white spaces in between words ,Removing “\n” and Removing NonEnglish character.

Vectorization
In tokenization we split the raw text into small chunks of words or sentences and we call this tokens.
For this we will be using the Fast-text vectorization technique. In this technique we use character-level embeddings instead of word level.
We use this vectorization technique to convert words into values that the machine can easily understand it.

Model Training
Now in order to train our model we split the data into 70/20/10 for
train set , validation set , test .

After all the prepossessing work We will use the hybrid model of Bilstm. We basically feed the data into our model in order to train it.
And later use it to predict values of the various labels that we provided
beforehand

Model Prediction
Now we provided an input text to the model and obtained an output Array that tells us if that particular tag is present in the sentence of not.We also plotted a graph to tell us about the loss in data during the prediction

Model Evaluation
The model was evaluated based on precision, recall and accuracy


## Results
In this project , we present a combination of convolutional and bidirectional neural network .The combined BiLSTM model gives good results over the long text, since it benefits from the  BiLSTM’s characteristic to learn long-term bidirectional dependencies of the text
The accuracy was found to be 88% 

