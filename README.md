# UMBC DATA SCIENCE Capstone project

# Author: Yaswanth Reddy Annapureddy

# Project: Binary Image Classification using CNN Model

## PROBLEM STATEMENT
Solid waste management is one of the world's most severe problems. Solid waste is produced by a variety of human activities including residences, businesses, farms, and other industries, and poses serious dangers to the environment and the general public's health. When ignored, it may lead to a threat to the ecosystem. Segregation is one method of managing solid waste. Different sorts of solid trash are sorted to accomplish this. Therefore, to appropriately dispose of the garbage, it is crucial to explicitly identify its type. The problem is 'how do we manage this waste, while we can't use it anymore?'. Several nations have issues related to waste because the waste production rate is not at par with its management efforts. Many people just dispose of mixed waste in dump sites because they are unaware of the effects of garbage that has not been properly segregated before it is disposed of. Kitchen garbage, agricultural waste, and human and animal waste are all examples of biodegradable waste that can be broken down biologically by live microbes. Non-biodegradable wastes, on the other hand, are wastes that cannot be broken down biologically. Plastic, metal, glass, etc. are all included. This is the reason why managing non-biodegradable trash through various technologies and solutions has gained more significance in the modern day. To categorize waste into biodegradable and non-biodegradable types, this work offers a solution for the stated problem using machine learning models, tensor flow, and convolutional neural networks. We have taken more than 150k images of biodegradable and non-biodegradable items to train the model.

## OBJECTIVE
Our aim is to classify the waste with automation as a trained model at its base to quickly separate both so that they can be sent separately to either recycling or dump accordingly.
We aim to regularize the classification of trash for environmental purposes.
Cities and metropolitan areas can implement this model to collect data on how citizens are using the recycling facilities, and how to improve the service.

## SOLUTION
we have taken a total of 150K images in each category and trained a CNN model with Keras to test the accuracy and efficiency of the model.
Used traditional deep learning techniques like tensor flow, and Keras.
If the model is paired with an AI GPU with Open cv, we can immediately classify the trash and optimize the recycling process.
One more advantage is that cleaning robots can quickly identify and classify waste accordingly.

## DATASET
Our dataset contains a total of more than 150K images in both bio-degradable and non-biodegradable materials, sourced from the Kaggle open dataset. Link: https://drive.google.com/file/d/1RaXQcHUcVveDjVa09k5Zhn5ZanOuykBY/view?usp=share_link

## Model:
The input for the model will be Image and the Label/Output is the classification of the image. The model will be trained using CNN-RNN algorithms. This is a kind of encoding-decoding. the encoder here will be Neural networks such as LSTM and the decoder will be the CNN as it will detect the information from the image.
