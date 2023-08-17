# My-GAN
My first ever rendition of Generative Adversarial Networks (GANs) which are a deep-learning-based generative model. GANs learn to generate new data with the same statistics as the training set. It consists of two networks, the Generator & the Discriminator, playing an adversarial game against each other. The Generator produces fake data to tick the the Discriminator whereas the Discriminator inspects the fake data & determines whether if it is real or fake. They are randomly initialised in the beginning & are trained simultaneously.


## Demo
I ran it for 100 Epochs using the [MNIST dataset,](https://en.wikipedia.org/wiki/MNIST_database) using the Adam Optimizer. The following shows a series of images produced by the generator as it was trained.

![epochshowcase](https://github.com/omcodedthis/My-GAN/assets/119602009/da0a082b-0c38-4aa6-bb61-2539275aa8f4)

The images begin as random noise, and increasingly resemble hand written digits similar to the MNIST dataset over time.

## Adam vs SGD
The Adaptive Moment Estimation (Adam) Optimizer & Stochastic gradient descent (SGD) are optimization techniques used to improve the model's performance. Below shows the data generated after 30 Epochs using both optimizers.

![adamvsSGD](https://github.com/omcodedthis/My-GAN/assets/119602009/9c76189a-02be-48d0-b4b8-ca5a84c7760d)

Since the number of Epochs is small, I went with the Adam Optimizer as it tends to converge faster compared to the SGD Optimizer.


## Getting Started
* Get a Google Account [here](https://www.google.com/account/about/) to use Google Colab.

* Test it using this [Google Colab Notebook.](https://colab.research.google.com/drive/1JlCd-EC7AatYjlFO1jLHTA80jKz6cnXr)

Note that the maximum number of Epochs is set to 40 in the notebook. Using a T4 GPU, it would take around 14 minutes for it run completely. The output from a `max_epochs` value of 40 has been included the notebook for easy viewing.
