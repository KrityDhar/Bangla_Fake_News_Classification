
Bangla Fake News classification using Machine Learning models
-------------------------------------------------------------


Problem Statement:
------------------
Nowadays, everything is getting digitalized. So, with the blessings of modern technology, people can read news of the whole world through different kinds of online news portals. A large number of people in our country now read online news portals in Bengali. Among these news portals, there also have some fake news and real news. But, in maximum time mass people can’t discriminate between this two. That’s why it is necessary to classify fake news and real news. In this project, we use different kinds of machine learning models such as Random Forest, Logistic Regression, KNN, and Decision Tree for the dataset named “BanFakeNews” to classify whether the news is real or fake. Among these models, Logistic Regression comparatively performs better gaining 92%.


Dataset:
--------
The provided dataset contains around 8.5k news data on the different news portals. Between these, around 7k are authentic, and around 1k are fake news. The fake news is labeled with 0 and the real news is labeled with 1.
 
![Capture](https://user-images.githubusercontent.com/115772405/214100462-5c2c5722-f908-47df-b69a-5086909d67e8.PNG)

                                              Fig. 1. Histogram of frequency and content length


Approach:
---------
 The dataset contains raw data and we have cleaned this dataset by removing stop-words, special characters, and punctuations in the pre-processing stage. For separating every word, we have used here tokenization. Then we extracted the features from the news data using TF-IDF. The following diagram is for workflow:
 
![Capture 1PNG](https://user-images.githubusercontent.com/115772405/214100292-d20cac80-5399-43a3-b94d-6d47e01cfa52.PNG)


                                               Fig.2. Block Diagram of Fake News Classification

We have classified the news according to the following steps:

Step 1:  Load the dataset.

Step 2:  Remove stop words, punctuations, and special characters.

Step 3:  Use TF-IDF for feature extraction.

Step 4: Then split the dataset into 70% and 30% where 70% is for training and 30% is for testing part.  

Step 5:  Use Machine learning models (Random Forest, Logistic Regression, KNN, Decision Tree).

Step 6:   Calculate Recall, Precision, F1 Score, and Accuracy for every model. From these Metrics, we have got the best model for which we have got the best accuracy.


![Capture3](https://user-images.githubusercontent.com/115772405/214100318-b03035af-4e06-434e-8e5b-104952133ce3.PNG)

                                          Fig.3. Performance Table of Machine Learning Models


Conclusion:
-----------
Our main aim is to classify fake news and real news from different online portals. Here, the Logistic Regression model performs better than the other models to classify fake and real news. We can improve the accuracy by increasing the dataset and using deep learning models in the future.


