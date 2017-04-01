# Advanced Lane Finding Project

In this project, the goal is to write a software pipeline to identify the lane boundaries in a video.

## Project Overview

The goals / steps of this project are the following:

* Compute the camera calibration matrix and distortion coefficients given a set of chessboard images.
* Apply a distortion correction to raw images.
* Use color transforms, gradients, etc., to create a thresholded binary image.
* Apply a perspective transform to rectify binary image ("birds-eye view").
* Detect lane pixels and fit to find the lane boundary.
* Determine the curvature of the lane and vehicle position with respect to center.
* Warp the detected lane boundaries back onto the original image.
* Output visual display of the lane boundaries and numerical estimation of lane curvature and vehicle position.

[//]: # (Image References)

[video1]: ./demo.gif "Video"

### Result

![alt text][video1]

Please refer to [solution.ipynb](https://github.com/Everhusk/Self-Driving-Car-Engineering/blob/master/P4%20-%20Advanced%20Lane%20Finding/solution.ipynb) for the code and steps used to come up with a solution.  

---

### Future Improvements

A few placed involved hardcoding parameters (warp perspective, binary thresholding coefficients), these could be automated by using some form of optimizer based on the imput camera angles etc. Automating the binary threshold coefficients would lead to a much more robust lane finding algorithm in all terrains (snow, rain, etc.). Lastly, the smart line detection algorithm could use frames past the previous one to better extrapolate values for the current frame.
