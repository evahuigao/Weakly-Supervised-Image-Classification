# Weakly-Supervised-Image-Classification

## Introduction
Weakly supervised learning is an essential problem in computer vision tasks, such as image classification,
object recognition, etc., because it is expected to work in the scenarios where a large dataset with clean
labels is not available.


## Goal
• Implementing a noise regularizing CNN model and Weakly supervised GAN that can classify images with noisy labels.

## Project outline:
• For training data: Split the dataset into clean labels (<10%) and dirty labels (>90%). For the dirty labels, randomly shuffle the labels
among images.
• Replicate the noise regularizing model shown
in https://openaccess.thecvf.com/content_CVPR_2019/papers/Hu_Weakly_Supervised_Image_Classification_Through_Noise_Regula
rization_CVPR_2019_paper.pdf and train your dataset.
• Replicate the WSGAN shown in https://arxiv.org/pdf/2111.14605.pdf and train your dataset.
• Compare the performance on your test data and explore the difference between two methods.
• Develop a model which can leverage the adversarial learning architecture in GAN to replace the regularizing network to improve
performance. Test your model by change the split level for clean labels starting from 10% and getting down as low as 5%. Find the cut
off for which the model performance stops improving.
• Dataset: https://pytorch.org/vision/stable/generated/torchvision.datasets.FashionMNIST.html (or any multilabel dataset of your
choice)
