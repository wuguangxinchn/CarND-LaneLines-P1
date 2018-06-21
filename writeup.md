# **Finding Lane Lines on the Road** 


---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report

---

### Reflection

### 1. Short pipeline description 

My pipeline consisted of following steps: 

First, I converted the images to grayscale, then applied Gaussian Blur and Canny Edge Detection ("Blur" is widely used to reduce noise before Edge Detetion).  

After that, I applied image mask to only keeps the region of the image defined by the polygon. then use Hough transform to get the image with hough lines drawn.  

Finally, overlay the output and original images.


### 2. Identify potential shortcomings with your current pipeline

In this project there is still much space to improve, especially the draw_lines() function. Will update later. 


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to refine draw_lines() function, and another potential improvement could be to make it more robust, especially there are other obvious lines in the images.  
