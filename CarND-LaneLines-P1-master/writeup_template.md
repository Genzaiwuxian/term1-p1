# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

the pipeline are:

- read image from floder
- change RGB image into gray_scale image
- do the gaussion_blur, and delete the noise
- find the Region of Interest, and do the houghline plot
- weighted the recongized red lane line with initial image
- import moviepy function,etc
- process the image into movie
- save the movie and show in HTML

### 2. Identify potential shortcomings with your current pipeline

- some small or can be called as noise white/yellow point is identified as lane line, next it's better to tuning the parameters (like threthold , minimum/maximum_line_len)
- moviepy model import error, finally i add the sys path and absolute path into pipeline to solve this problem, maybe it's version problem, try install function/model based on one environment, like anaconda.
- optional challanges missed casued of time, try again after finished P5 Term1.


### 3. Suggest possible improvements to your pipeline

- during my work with challange, many another lines(no the lane line) is detected. 
- 1st i can make some code to filler the small lines
- but i can't think other countermeasures to solve this questions based on the method in this lesson, maybe the Deep learning of CNN some else can solve this questions.
