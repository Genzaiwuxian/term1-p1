# term1-p1



## Lane Finding Pipeline
the pipeline are:
- read image from floder
- change RGB image into gray_scale image
- do the gaussion_blur, and delete the noise
- find the Region of Interest, and do the houghline plot
- weighted the recongized red lane line with initial image
- import moviepy function,etc
- process the image into movie
- save the movie and show in HTML

## Final result
- the lane line (white/yellow) can be successed idetificated, and from image into a video as output
- right and left lane line can be successed identificated, and final annotations of video have the segmented and solid laneline in it
![image](https://github.com/Genzaiwuxian/term1-p1/blob/master/CarND-LaneLines-P1-master/solidWhiteCurve_img_output.jpg)
![image](https://github.com/Genzaiwuxian/term1-p1/blob/master/CarND-LaneLines-P1-master/solidWhiteRight_img_output.jpg)
![image](https://github.com/Genzaiwuxian/term1-p1/blob/master/CarND-LaneLines-P1-master/solidYellowCurve_img_output.jpg)


## Reflection
  - some small or can be called as noise white/yellow point is identified as lane line, next it's better to tuning the parameters (like threthold , minimum/maximum_line_len)
  - moviepy model import error, finally i add the sys path and absolute path into pipeline to solve this problem, maybe it's version problem, try install function/model based on one environment, like anaconda.
  - optional challanges missed casued of time, try again after finished P5 Term1.
 
