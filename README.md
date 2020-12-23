# Covid-Detection-using-X-rays

# Introduction  

We are aiming to predict the covid nature of a person with the help of the chest X - Ray.The ongoing flare-up of the novel Covid illness (nCOVID-19) has contaminated a large number of individuals and slaughtered a few people all over the world. The World Health Organization (WHO) has proclaimed this plague a worldwide wellbeing crisis. nCOVID-19 is brought about by a profoundly infectious infection named serious intense respiratory condition Covid 2 (SARS-COV-2) in which transmission of infec-tion can even happen from the asymptotic patients during the brooding time frame according to the master's conclusion, the infection predominantly taints the human respiratory parcel prompting extreme bronchopneumonia with indications of fever, dyspnea, dry hack, weariness, and respiratory disappointment, 

# Motivation 
The motivation of our project is to develop an efficient model which can easily verify the covid status of a person, follow his tracks and easily help us to quarantine the person infected to avoid the spread of Covid-19 and overcome this pandemic.

# Background 

A Convolutional Neural Network (CNN) is a class of feed-forward neural organizations. CNN is based on top of four key thoughts: neighborhood association, sharing loads, pooling, and utilization of various layers. The engineering of a regular CNN is made out of these layers; in an initial segment: convolution layer, ReLU (Rectified Linear Units), pooling layer and in a subsequent part: completely associated layer, misfortune layer .

The convolution layer applies a bunch of discrete convolutions on the yield of the past layer. Every convolution is finished utilizing a portion (likewise called: veil, channel bank) and creates 
a 2D include map. This layer is additionally observed as a layer with neighborhood associations so a neuron is associated uniquely to neurons of the past layer in a similar locale. Neighborhood associations give the capacity to the layer to distinguish nearby examples from the past layer. 

# Data Collection
 
We have collected our dataset from Github (https://github.com/ieee8023/covid-chestxray-dataset) and Kaggle (https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia websites). The data has been preprocessed and normalized to suit our model. It has each image of size 224 * 224 * 3. It consists of around 392 images and is of more than 181 Mb in size. The dataset does not contain proper data split for training purposes, so we perform our own split
(9 : 1). The dataset has been used for various research papers.

# Experimental Design

We have designed our network architecture by own and experimented with different activation functions, layer and have arrived at a better result than the original model on the chosen dataset. Although, original model was a model can also handle that. Before start the training we also normalise our image parameters so that it will take less computation and train fast.

The pooling layers is by maximum elements from features will reduce dimension features by half also called as sub sampling followed by flattening layer to reduce image to one dimensional vector to fed into neural network.

# Results and Comparison
Our results indicate that this approach can lead to COVID-19 detection from X- Ray images. We implemented three models for the purpose of Covid Detection using X-rays. We achieved an accuracy of 88% using Artificial Neural Network, 93% using Convolution neural network and 62% using Resnet50 model (Transfer Learning).We got area under the ROC-curve as 0.96 using Artificial Neural Network, 0.98 using Convolution Neural Network, 0.79 using Transfer Learning.
Multilayer Perceptron :

Class
Precision
Recall
F1-Score
Covid - Positive
1
0.76
0.86
Covid - Negative
0.79
1
0.88

 
 Accuracy = 0.88
Area under ROC Curve : 0.96

Convolution Neural Network :


Class
Precision
Recall
F1-Score
Covid - Positive
0.92
0.96
0.94
Covid - Negative
0.93
0.87
0.90

 
 Accuracy = 0.93
Area under ROC Curve : 0.98

Transfer Learning :

Class
Precision
Recall
F1-Score
Covid - Positive
0.83
0.26
0.40
Covid - Negative
0.59
0.95
0.73

 
 Accuracy = 0.62
Area under ROC Curve : 0.79
 
 Conclusion  

Hence, by experimenting over models on the chosen architecture on the chosen dataset. We can conclude that ,We have introduced some underlying outcomes on recognizing COVID-19 positive cases from chest X-Rays utilizing a profound learning model. the main freely kept up instrument for grouping of COVID-19 positive X-beams, on a similar chest-xray-pneumonia dataset. The outcomes look encouraging, however the size of the freely accessible dataset is small. We intend to additionally approve our methodology utilizing bigger COVID-19 X-beam picture datasets and clinical preliminaries
