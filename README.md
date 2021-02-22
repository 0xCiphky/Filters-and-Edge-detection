# Filters and Edge detection
Assignment 2: Filters and Edge detection

FILTERS
Part I (10%) Computing linear filters in scikit-image/python. Before it said 20% but this would make the total marks 110%

Read a grayscale image moon.png. 
Filter the grayscale image with the following filters.
Display results.
Create a 3-by-3 matrix and write your own code to implement these filters: (You cannot use any built-in functions from any library for this.)
1) Laplacian Filter

2) [0,0,0]
    [0,1,0]
    [0,0,0]

3) [0,0,0]

    [0,0,1]

    [0,0,0]

4) compute Im + (Im - Im * average_filter) # where * is a convolution operation and Im is moon.png.

Part II (10%) Median and Gaussian filters

Read noisy.jpg corrupted with salt and pepper noise.
Apply a median filter to remove the noise.
Apply a Gaussian filter to the same noisy image.
You can use any scikit-image functions you like.
Which filter was more successful?
Part III (30%) An application of filtering in scikit-image: Simple image inpainting.

Write a program in scikit-image/Python to accomplish a simple image inpainting. This example and demo were shown in the lecture.

Use damage_cameraman.png and damage_mask.png.

It is an iterative algorithm. At every iteration, your program (a) blurs the entire damaged image with a Gaussian smoothing filter; then (b) with help of the mask image, restores only the undamaged pixels. Repeat these two steps (a) and (b) a few times until all damaged pixels are infilled.

Edge detection
Part IV : Edges (25%)

Read the gray scale image ex2.jpg. Display the image. Compute gradient of the image (both the horizontal derivative and vertical derivative) by Sobel operators. You can find more details about the Sobel filter in here and here. To compute the derivatives, you can use the functions skimage.filters.sobel_v and skimage.filters.sobel_h. Display the horizontal and vertical direction derivative images. Compute gradient magnitude image by suitably combining the horizontal and the vertical derivative images. Display the gradient magnitude image.

Part V: Canny edge detector (25%)

Read the gray scale image ex2.jpg and display it. Since the first step in Canny edge detection is Gaussian filtering, to understand the effect of Gaussian filtering, apply Gaussian filtering on the image and show the smoothed image.

Then, study the code provided here for Canny edge detection. Now do the followings:

1. To understand the effect of threshold values, fix sigma = 1.0, use matplotlib.pyplot.subplot to plot the following 4 figures together and see their difference : low threshold = 25; low threshold = 50; high threshold = 150; high threshold = 200.

2. To understand the effect of sigma value, fix low_threshold=50 and high_threshold=150, use matplotlib.pyplot.subplot to plot the following 4 figures together and see their difference : sigma =  1.0; sigma = 1.5; sigma = 2.0; sigma = 2.5.
