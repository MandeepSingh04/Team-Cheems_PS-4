# Team-Cheems_PS-4
## Our understanding of the problem statement
- The problem statement focuses on the image based recognition of fish species and a rough estimation of their proportion when they are brought to the harbours as a harvest. 

- Since the main issue is with classification, so we came with an application which is integrated with a convolutional neural network based machine learning model in order to recognize a particular fish species.

- And to fulfil the demand of problem statement, our model also classifies fish species in different categories and estimating their market price.

## Our idea & approach
Keeping in view the feasibility, simplest platform should be developed keeping the accuracy as high as possible.
That turn out to be an Android App having Machine learning model ( CNN ) to ensure both.

## Motivation 
The major reason was the problems faced by fisherman in harbour, lack of awareness of market information, uncertain quality of fish, faulty measurement system. They do not have any specific way to have market information, places to sell the fishes etc. at just one click which result in huge loss.

## Economic feasibility
This complete implementation works on almost no cost from the user end. The user just need to download the app, capture the image and get details. Availability of android app is quite common and almost everyone has access to it now-a-days. 

# Technical Details
## DataSet 
The dataset is made available for the research purposes online by Oguzhan Ulucan. The dataset was formed a year ago.
This dataset contains 9 different seafood types collected from a supermarket in Izmir, Turkey for a university-industry collaboration project at Izmir University of Economics.
For each class, there are 1000 augmented images and their pair-waise augmented ground truths.
Each class can be found in the "Fish_Dataset" file with their ground truth labels.

The dataset includes, 
- gilt head bream, 
- red sea bream, 
- sea bass, 
- red mullet, 
- horse mackerel, 
- black sea sprat,
- striped red mullet, 
- trout, 
- shrimp image samples.

Created by O.Ulucan , D.Karakaya and M.Turkan.(2020) A large-scale dataset for fish segmentation and classification. In Conf. Innovations Intell. Syst. Appli. (ASYU)

## Model
We have used a type of convolutional neural network named MobileNet which uses depthwise separable convolutions. It significantly reduces the number of parameters when compared to the network with regular convolutions with the same depth in the nets. This results in lightweight deep neural networks and so works faster.

Various python libraries are used in this model like numpy, pandas, scikit-learn, tensorflow.

## Android app
The android app was built with tech stack java and xml using android studio. Java is used because it has platform independent feature and as android code is written once and to execute need to compile and optimise native code for better performance on various devices. It works faster for the large dataset and xml was used to declare layouts and java to provide logic.

## Deployment
Model was deployed to android app with the help of tensorflow lite mode. Keras will be used to generate a neural network model. Using lite, we will convert the model into tflite format for Android.
