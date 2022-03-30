# Colourize-BW-photos

The aim was to create an autoencoder to learn the function of converting a grayscale image into an RGB image. For this, an encoder-decoder model is used, which is an advanced version of CNN Architecture.

The methodolgy is precisely and wonderfully explained by [Emil Wallner](https://emilwallner.medium.com/colorize-b-w-photos-with-a-100-line-neural-network-53d9b4449f8d) 

The input image is seen as a grid representing a black and white image. It outputs two grids with color values. Between the input and output values, we create filters to link them together. That is the convolutional neural network. To train our network, we use the colored images from our dataset. The RGB colors are converted to Lab color space and then the predicted values and the real values are mapped within the same interval.
Lastly, the grayscale layer is copied from the test image, and two-color layers area dded to the RGB canvas. The resulting array of pixel values is converted into a
picture and finally outputted.

-- The following code is inpired, adapted, and learnt from [Emil Wallner](https://emilwallner.medium.com/colorize-b-w-photos-with-a-100-line-neural-network-53d9b4449f8d) and [Edureka!](https://www.youtube.com/watch?v=lLy0sRmxVvo)
