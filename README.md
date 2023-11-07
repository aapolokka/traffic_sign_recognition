# Traffic Sign Recognition using Convolutional Neural Networks

## Introduction

One of the most critical step for safer autonomous vehicles is to recognize traffic signs. This project will focus on the traffic sign recognition performance using three different convolutional neural network (CNN) architectures. The three different CNN architectures that are used in this work are LeNet, AlexNet, and VGGNet. I have written a paper from this project, which can be found from repository.

## Data

Datapoints were gathered from the German Traffic Sign Recognition Benchmark ([GTSRB](https://benchmark.ini.rub.de/gtsrb_news.html)) dataset. The GTSRB dataset consists of 39209 training images, which are divided to 43 different classes. These classes include different speed limit, dangerous, and order traffic signs. The GTSRB dataset consists consist also, 12629 unlabeled testing images for evaluating the performance and quality of the different CNN architectures.  

Also, the best performing CNN model was tested the dataset that was created by me (images are shown in images_folder). The dataset was created by taking images of different traffic signs, and then classifying these to the correct classes. This dataset includes 48 training images, which are divided to 4 different classes equally. These classes are no parking, triangle, walkway, and pedestrian crossing traffic signs. The dataset also includes 10 different unlabeled testing images

## Results

| Model  | LeNet (GTSRB) | AlexNet (GTSRB) | VGGNet (GTSRB) | VGGNet (own dataset) |
| ------ | ------ |------ | ------ | ------ | 
| Accuracy: | 0.938 | 0.970 | 0.973 | 0.894 |

As shown in table above, the best performing network is the VGGNet, which was expected since it solves the AlexNet’s problem of including too many hyper-parameters and is more precise than simpler LeNet. The worst performing network was VGGNet with writer’s own dataset. Also, this behavior was expected since the dataset was so small, only including 12 images in each 4 classes. 

## Required external packages

```
Tensorflow
Keras
numpy
pandas
PIL
sklearn
```
