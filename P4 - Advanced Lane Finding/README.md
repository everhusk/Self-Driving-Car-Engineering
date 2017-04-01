# Advanced Lane Finding Project

In this project, the goal is to write a software pipeline to identify the lane boundaries in a video.

## Project Goals / Steps

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

[image1]: ./undistort_output.png "Undistorted"
[image2]: ./test_images/test1.jpg "Road Transformed"
[image3]: ./binary_combo_example.jpg "Binary Example"
[image4]: ./warped_straight_lines.jpg "Warp Example"
[image5]: ./color_fit_lines.jpg "Fit Visual"
[image6]: ./example_output.jpg "Output"
[video1]: ./demo.gif "Video"

### Solution

Please refer to solution.ipynb for the code and steps used to come up with a solution.  

### Demo (video)

![alt text][video1]
---

### Future Improvements

The calibration methods could be improved a bit and some tuning parameters need to be adjusted (not much time was spent on it).
