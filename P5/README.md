#**Advanced Lane Finding**

By: Sukhveer Sanghera

# Problem Description

Write a software pipeline to detect vehicles in a video stream. [1]

## Goals

* Perform a Histogram of Oriented Gradients (HOG) feature extraction on a labeled training set of images and train a classifier Linear SVM classifier
* Optionally, you can also apply a color transform and append binned color features, as well as histograms of color, to your HOG feature vector.
* Note: for those first two steps don't forget to normalize your features and randomize a selection for training and testing.
* Implement a sliding-window technique and use your trained classifier to search for vehicles in images.
* Run your pipeline on a video stream (start with the test_video.mp4 and later implement on full project_video.mp4) and create a heat map of recurring detections frame by frame to reject outliers and follow detected vehicles.
* Estimate a bounding box for vehicles detected.

# Solution

## High Level Overview

The pipeline used to solve this problem consists of the following 5 steps:

1. Convert images to grayscale
2. Draw the lines

---

## Potential Shortcomings

One potential shortcoming would be what would happen when ...
Another shortcoming could be ...

## Future Improvements

A possible improvement would be to ...
Another potential improvement could be to ...

# Referenecs
[1] https://github.com/udacity/CarND-Advanced-Lane-Lines
