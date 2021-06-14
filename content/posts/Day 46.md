---
title: "Day 46"
date: 2021-06-14T12:02:01+05:30
draft: false
---

Day 46

# Day 46

* Mini batch and its uses
* The NaN trap
* Optimizers in Tensorflow

Mini batch is taking a batch size lower than the selected batch size. It is more efficient and quicker to calculate loss for mini batches than the whole training data.

When training the model, if one of the numbers becomes NaN and it leads to many or all NaN's to the other numbers in a model. This is the NaN trap.

Optimizer is a specific implementation of the gradient descent algorithm in a model. Types: AdaGrad and Adam

Gradient Descent - A technique to minimize loss by computing the gradients of loss with respect to the model's parameters, conditioned on training data. Informally, gradient descent iteratively adjusts parameters, gradually finding the best combination of weights and bias to minimize loss.