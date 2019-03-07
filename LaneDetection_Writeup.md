# Self Driving Car Lane Detection

---
### Goals:

The goals of this project are as follows:

* Provide a pipeline in order to detect lanes on a road
* Output an overlay of the lines detected onto the images provided
* The ability to provide lane lines overlay on a video stream

---

### 1. Reflection

Using grayscale transformation and a gaussian blur, this allows the application to remove the noise on an image.

By using the canny edge detection algorithm, it detects the maximum value of given thresholds in an edge within an image.

Determining a polygon to mask on an image will find a region of interest and fill the pixels inside the masked region defined by vertices.

The hough transformation has a set of parameters in which they are used by aligning points on an image that create lines.

By using slope intercept parameters, we can average out the lines detected and better overlay the lines on an image when we use the draw_lines function.



### 2. Potential shortcomings within current pipeline


One potential shortcoming would occur with the lanes on the road curving through a turn. The ability to detect the lanes while making a turn have not yet been resolved. 


### 3. Suggest possible improvements to your pipeline

A possible improvement theory in the current pipeline would be to determing a different polygon mask parameter with a smaller region on the images and video stream in order to better detect lines on a curved road.
