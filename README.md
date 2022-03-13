# Brain-Tumor-Detection
The idea of the project was to reproduce and improve the result of a [scientific publication](https://ieeexplore.ieee.org/abstract/document/8934561) on Brain tumor detection using CNN (Convolutional Neural Network) with MRI images.

# Fluxogram of the Process Presented
![Fluxogram image](https://user-images.githubusercontent.com/49374221/154573946-a21cb310-b1ca-4f07-8597-57f929b77439.png)

# Convolutional Neural Network(CNN)
The CNN will extract features maps from each image through an operation called convolution which works by taking a cluster of pixels and multiplying each pixel with the
convolutional filter corresponding (the one that the neural network learn) and making a sum of the multiplyed pixels, repeating this process for all the pixels in a
given image, the result will be a feature map. The feature map will be aplied to another test image and used like a feature identifier, a convolution operation will be 
made and for avery cluster of the test image the filter will be aplied, if the test image has the given caracteristics the result will be a high number ,making possible 
to identify, in this case, what is or what is not a brain tumor.

![gif](https://user-images.githubusercontent.com/49374221/154580423-86b2500c-815c-4186-882c-ee37c84043d1.gif)

# Max Pooling
The maximum pooling layer is a compression layer, reducing the computation of all the convolution steps. The max pooling works by taking a cluster of a given size and 
shifting around the image and for each movement either taking the avarage of the values or choosing the max value of the cluster.

![MaxPooling](https://user-images.githubusercontent.com/49374221/154583764-f7cb4209-7682-4410-b406-55d1b17cbe84.gif)

# MRI images
The database contains 4600 different images, with various sizes and shapes taken from [Kaggle](https://www.kaggle.com/), with MRI images classified as healthy or unhealthy.
## Healthy 
![Mri Healthy](https://user-images.githubusercontent.com/49374221/154584763-4cc6bae4-ec5a-4606-9bd7-ded4beb847dc.png) 

## Unhealthy
![MriImages](https://user-images.githubusercontent.com/49374221/154584440-760db88e-87e9-4054-89c6-46702bea4b73.png)

# Results

### 1º Plot accuracy x accuracy on validadion dataset (per epoch)
![AccuracyPlot](https://user-images.githubusercontent.com/49374221/154586311-3aedeee2-0759-4c55-82be-e63c39d926df.jpg)
### 2º Plot comparing de loss x loss on validadion dataset (per epoch).
![loss plot](https://user-images.githubusercontent.com/49374221/154586652-2cb0fe36-5066-4288-a4e3-068d99d92000.jpg)



