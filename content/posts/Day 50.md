---
title: "Day 50"
date: 2021-06-14T12:02:01+05:30
draft: false
---

Day 50

# Day 50

* Convolutional Operation
* MNIST
* Size Invariance

The following two-step mathematical operation:

* Element-wise multiplication of the convolutional filter and a slice of an input matrix. (The slice of the input matrix has the same rank and size as the convolutional filter.)
* Summation of all the values in the resulting product matrix.

For example, consider the following 5x5 input matrix:

Now imagine the following 2x2 convolutional filter:

Each convolutional operation involves a single 2x2 slice of the input matrix. For instance, suppose we use the 2x2 slice at the top-left of the input matrix. So, the convolution operation on this slice looks as follows:

A convolutional layer consists of a series of convolutional operations, each acting on a different slice of the input matrix.


A public-domain dataset compiled by LeCun, Cortes, and Burges containing 60,000 images, each image showing how a human manually wrote a particular digit from 0–9. Each image is stored as a 28x28 array of integers, where each integer is a grayscale value between 0 and 255, inclusive.

MNIST is a canonical dataset for machine learning, often used to test new machine learning approaches. For details, see The MNIST Database of Handwritten Digits.

In an image classification problem, an algorithm's ability to successfully classify images even when the size of the image changes. For example, the algorithm can still identify a cat whether it consumes 2M pixels or 200K pixels. Note that even the best image classification algorithms still have practical limits on size invariance. For example, an algorithm (or human) is unlikely to correctly classify a cat image consuming only 20 pixels.