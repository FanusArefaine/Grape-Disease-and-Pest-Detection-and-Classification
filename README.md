# Grape-Disease-and-Pest-Detection-and-Classification
A project to detect and classify Grape Diseases and Pests


## Motivation

Although grapes are among the top 20 most produced agricultural commodities, the demand has been exceeding production rate. Likewise, the domestic demand of wine exceeds the efforts of growing grape production in the United States of America. In 2018, the grape farm was valued at USD 167 billion and estimated to grow with a CAGR of 7.1% within the period 2019-2024, reaching USD 254.29 by 2024. Despite the efforts made to expand and increase production, grape industry faces major loss due to diseases and pests. The executive director of the Washington Wine Growers Association Vicky Sharlau once quoted, “You can’t make good wine with bad grapes.” Disease and pest control have been one of the major challenges hindering production growth in the grape industry. This project, Grape Disease and Bug Detection and Classification, is a Deep Learning based model that addresses this challenge in the grape industry. This project is mainly focused on the detection and classification of certain diseases; Black measles, Black rot and Leaf blight, and Bugs; Mealybug and Phylloxera. This project utilizes ResNet50, a deep learning model, to provide optimal performance in detection and classification of grape diseases and bugs. The deep learning model, ResNet50 is tuned to achieve model independent optimal performance and the final outcome evaluated based on the accuracy value. 


## Dataset

The dataset consists of 6 classes that cover both diseases and bugs, and healthy data. In which, diseases contain black measles, black rot, and leaf blight; pests contain phylloxera and mealybug. Total images of the 6 classes is around 13,400.

One of the most common and vicious bugs in Napa Valley, California grape farms is mealybug. Although it has not been easy to get a good quality image dataset, I have hand-picked mealybug images from google images for the project. More images of the current pests and more kinds of pests also will be added into this dataset if good dataset resources are found.



## 2. Resnet50


### Introduction

Residual Neural Network for Image Classification Tasks: It is an image classification neural network commonly known as ResNet. In this project I used a ResNet model with 50 layers known as ResNet50. The ResNet50 model involves deep networks to extract low, middle and high-level features and classifiers in an end-to-end multi-layer fashion.


### Architecture

![image](https://user-images.githubusercontent.com/56777455/86096930-cd2f0f80-ba68-11ea-8e74-4c1ec5b532f1.png)


ResNet was introduced by Microsoft to address a degradation problem when deeper networks start to converge. With the increase of network depth, accuracy gets saturated and then degrades rapidly. While overfitting is not the cause for such degradation, and adding more layers worsens the problem. Hence, ResNet was schemed to address such problems.

In ResNet, every stacked layer is fitted into residual mapping, instead of directly fitting into a desired underlying mapping. The formation of F(x)+x can be schemed by forward feeding neural networks with shortcut connections. Shortcut connections can be shown above as the lines skipping one or more layers. In ResNet, identity mapping is performed by the shortcut connections and their outputs are added to the outputs of the stacked layers.



## Advantages of ResNets

- ResNet model is less likely to suffer from vanishing gradient problem when trained for much deeper network compared to plain networks

- ResNets avoid the high training and testing error when trained for deeper networks which happen with ‘plain’ networks.

- Given a ResNet model has a much deeper network, the model size is significantly low when compared with any other model of the same depth.

- Unlike plain networks, ResNets can easily gain accuracy from increasing depth and converge faster than other plain counterparts. In ILSVRC-2015, ResNet won first place achieving a top-5 validation error of 4.49%.
