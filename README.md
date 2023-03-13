# Sports Cars Classifier

Data science project example using deep learning for image classification.

## Overview
This is a data science project that demonstrates the use of deep learning for image classification. It is based on a [video](https://www.youtube.com/watch?v=vy-R4oUZaC8&t=1142s&ab_channel=KenJee) tutorial by [Ken jee](https://github.com/PlayingNumbers), where he builds a [ball classifier](https://github.com/PlayingNumbers/ball_image_classifier) that identifies balls from different sports with 94% accuracy. 

The main idea was to replicate the project to learn and apply the basics of deep learning and use a different data set to see how well the model can be trained using more complex objets (sports cars in this case).  After using transfer learning on a Convolutional Neural Network (CNN) trained on resnet34 to classify sports cars based on their brand, I was able to get the model to predict the brand of the car with 94% accuracy.

![](https://raw.githubusercontent.com/SantiagoCuello97/Sports-Cars-Classifier/main/matrix_results.png)

## Data
I used the [FatKun Batch Download Image](https://chrome.google.com/webstore/detail/fatkun-batch-download-ima/nnjjahlikiabnchcpehcpkdeckfgnohf?hl=en) chrome extension to download the sports cars images from Google. The dataset consists of a collection of sports cars images from 10 different brands. The dataset is available [here](https://drive.google.com/drive/folders/10AdU9eoJQTaoZ164-CIR26RaHwrpXYFG?usp=sharing), along with the two trained models.

## Notes
Few corrections had to be done from Ken's project since some of the things he used were available in the previous version of Fastai (v1), but not in the latest one.

For example, `ImageDataBunch.from_folder` was available before but has now been replaced with `ImageDataLoaders.from_folder`. More info can be found here: [FastAi - Vision Data](https://docs.fast.ai/vision.data.html#imagedataloaders.from_folder).


