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

Dataset parameters:
There are two parameters, namely:
1. Images
This column contains the local paths for the images which are fed into the model to pick up images
2. Label
This parameter consists of binary numbers 0 and 1. The 0 represents the biodegradable
image and 1 represents the non-biodegradable image.

## DATA COLLECTION AND MODEL MAKING
Data Collection Process:
The study's data set consists of 150K photos of trash divided into two categories:
"biodegradable" and "non-biodegradable." It is retrieved from the open-access Kaggle database.
Six categories make up the dataset: trash, glass, paper, cardboard, plastic, and metal. The
non-biodegradable class used some of these images that were gathered from the six categories,
and the biodegradable class used images of typical food waste.
Data Augmentation:
The performance of an algorithm improves with the amount of data it has access to. To
adequately train the machine learning models, the original dataset's relatively limited number of
photos needed to be augmented. Data augmentation is a way to increase the dataset's size and the
model's precision. By generating fresh data from the base data, data augmentation improves data.
Simply applying random changes to our images will improve the generalizability of our model.
Compressions, rotations, stretches, and even color shifts are examples of these transformations.
We have done this using ImageDataGenerator from tensorflow.keras.preprocessing.image.

# Training and Testing:
This is where the data is fit into the training set. Due to the callback's monitoring of the
validation set, the validation set is also passed. If the loss does not improve after two epochs as
specified in the EarlyStopping callback, the training process will be terminated by the callback.
In this scenario, you can define a large number of epochs.

## RESULTS
We got a total of 90 percent accuracy on the Training dataset and 95 percent accuracy on the
testing dataset.

## IMPACT OF THE PROJECT
If the model is used in AI-powered trash collectors or classifications, we can save millions of
trash from getting landfilled. If the bio and non-biodegradable materials are mixed with each
other, it's hard to classify and recycle the non-degradable. So if they are classified properly, we
can save tons of trash from going to landfills.

## REFERENCE
1.) Hanbal, I. F., Ingosan, J. S., Oyam, N. A. A., & Hu, Y. (2020). Classifying Wastes Using
Random Forests, Gaussian Naïve Bayes, Support Vector Machine and Multilayer
Perceptron. IOP Conference Series: Materials Science and Engineering, 803(1), 012017.
https://doi.org/10.1088/1757-899x/803/1/012017
2.) Atik, I. (2022). Analysis of Biodegradable and Non-Biodegradable Materials Using
Selected Deep Learning Algorithms. International Journal of Computer (IJC), 43(1),
48–59.
https://ijcjournal.org/index.php/InternationalJournalOfComputer/article/view/1939/712
3.) Bhansali, R. (2021, October 11). An Overview of Non-Biodegradable Waste
Management and Solutions. Organica Biotech.
https://organicabiotech.com/an-overview-of-non-biodegradable-waste-management-and-s
olutions/
4.) whoisslimshady. (2021, March 14). Introduction to Convolutional Neural Network With
Tensorflow and Keras. Geek Culture.
https://medium.com/geekculture/introduction-to-convolutional-neural-network-with-tens
orflow-and-keras-cb52cdc66eaf
5.) Derrick Mwiti, (2021, February 23). How to build CNN in TensorFlow: examples, code
and notebooks | cnvrg.io. https://cnvrg.io/cnn-tensorflow/
6.) What is Non-Biodegradable Waste: Define, advantages and disadvantages. (2020,
November 25). OkCredit Blogs - Business Ideas, Tips, Government Schemes & More.
https://okcredit.in/blog/what-is-non-biodegradable-waste/
