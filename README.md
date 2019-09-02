# **Finding Lane Lines on the Road** 


---

**Finding Lane Lines on the Road**

* Make a pipeline that finds lane lines on the road



[//]: # (Image References)

[image1]: ./test_images/solidWhiteCurve.jpg "before"
[image2]: ./test_images_output/solidWhiteCurve.jpg "after"

---

### Reflection

### 1. Create pipeline.

My pipeline consisted of 5 steps. 

1. Convert the images to grayscale
2. Apply a Gaussian Noise kernel
3. Canny transform to identify edge lines
4. Mask the image to only host lines visible
5. Apply Hough Transform to get lines

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by transform point to first order polynomial

Here is the picture show the transformation from beginning to end result: 

![alt text][image1]
![alt text][image2]


### 2. Shortcoming with my current pipeline


One potential shortcoming would be my pipeline more stable when dashed lanes on present 



### 3. Possible improvements to my pipeline

A possible improvement would be to increase robustness on curvy road situation.
