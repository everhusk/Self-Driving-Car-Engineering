# **Finding Lane Lines on the Road**

When we drive, we use our eyes to decide where to go. The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle. Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm. [1]

### Demo (white lanes):

Input:

![Example1](example1.gif)

Output:

![Demo1](demo1.gif)

### Demo (yellow lanes):

Input:

![Example1](example2.gif)

Output:

![Demo2](demo2.gif)

# Solution Overview

The goal was to detect lane lines using Python and OpenCV. For full details checkout the jupyter notebook.
Note: Lines may be straight, curved, or colored (i.e. yellow boundary lines, weather, TOD, etc.).

## Tools Available

* Color selection
* Region of interest selection
* Grayscaling
* Gaussian smoothing
* Canny edge detection
* Hough transform line detection
* Others

## Algorithm Pipeline

The pipeline used to solve this problem consists of the following 7 steps:

0. Read the image(s)
1. Convert the image(s) to grayscale
2. Apply a Gaussian noise kernal
3. Apply the Canny transform for edge detection
4. Mask the region of interest
5. Apply the Hough Transform
6. Approximate the left lane from positive slope lines, right from negative, and overlay them onto the image(s)

# Limitations

One potential shortcoming would be that when slopes of the lanes are both negative or positive the detection will fail. Also when the edge detection falls outside of the thresholds of the parameters (this needs to be more throughtly tested) the algorithm may not be able to detect the lane. Lastly, if there are obstacles obstructing the cameras view, it will fail.

# Future Improvements

A possible improvement would be to run an optimization function on the parameters used to tune it futher, rather than having to predict these. Smoothen out the video by incorporating previous frames into the current frames prediction would greatly enhance the display of the output, and correct for any outliers.

# Referenecs
[1] https://github.com/udacity/CarND-LaneLines-P1
