#**Finding Lane Lines on the Road**

# Problem Description

When we drive, we use our eyes to decide where to go. The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle. Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm. [1]

Given a road image/video:
![Alt text](/test_images/solidWhiteRight.jpg "Optional Title")

And produce an output line this:
![Alt text](/assets/laneLines_thirdPass.jpg "Optional Title")

Note: Lines may be straight, curved, or colored (i.e. yellow boundary lines, weather, TOD, etc.)

# Problem Solution

In this project, the goal is to detect lane lines in images using Python and OpenCV.

## Tools available

* Color selection
* Region of interest selection
* Grayscaling
* Gaussian smoothing
* Canny edge detection
* Hough transform line detection
* Others

## High Level Overview

The pipeline used to solve this problem consists of the following 5 steps:

0. Read the image
1. Convert the image to grayscale
2. Apply a Gaussian noise kernal
3. Apply the Canny transform for edge detection
4. Mask the region of interest
5. Apply the Hough Transform
6. Approximate the left lane from positive slope lines, right from negative, and overlay them onto the image
---

# Potential Shortcomings

One potential shortcoming would be what would happen when both slopes are negative or positive
When the edge detection falls outside of the thresholds
If there are obstacles on the bottom of the camera (i.e. in the challenge)

# Future Improvements

A possible improvement would be to run an optimization function on the parameters used to tune it futher
Smoothen out the video by incorporating previous frames

# Referenecs
[1] https://github.com/udacity/CarND-LaneLines-P1
