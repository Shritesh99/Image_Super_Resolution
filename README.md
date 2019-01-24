# Using The Super Resolution Convolutional Neural Network for Image Restoration

### This Repository is a part of [100DaysofMLCode challenge](https://github.com/Shritesh99/100DaysofMLCodeChallenge)

### Check out the Jupyter Notebook [here](https://github.com/Shritesh99/Image_Super_Resolution/blob/master/SRCNN.ipynb)

### Check out the project [here](http://shritesh99.github.io/Image_Super_Resolution/)

The goal of super-resolution (SR) is to recover a high resolution image from a low resolution input, or as they might say on any modern crime show, enhance!

To accomplish this goal, we will be deploying the super-resolution convolution neural network (SRCNN) using Keras. This network was published in the paper, "Image Super-Resolution Using Deep Convolutional Networks" by Chao Dong, et al. in 2014. You can read the full paper at https://arxiv.org/abs/1501.00092.

As the title suggests, the SRCNN is a deep convolutional neural network that learns end-to-end mapping of low resolution to high resolution images. As a result, we can use it to improve the image quality of low resolution images. To evaluate the performance of this network, we will be using three image quality metrics: peak signal to noise ratio (PSNR), mean squared error (MSE), and the structural similarity (SSIM) index.

Furthermore, we will be using OpenCV, the Open Source Computer Vision Library. OpenCV was originally developed by Intel and is used for many real-time computer vision applications. In this particular project, we will be using it to pre and post process our images. As you will see later, we will frequently be converting our images back and forth between the RGB, BGR, and YCrCb color spaces. This is necessary because the SRCNN network was trained on the luminance (Y) channel in the YCrCb color space.
