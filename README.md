# Motion-Detector-Using-OpenCV  <img alt="GitHub" src="https://img.shields.io/github/license/smahesh29/Motion-Detector-Using-OpenCV">

<h2>Problem Statement : </h2>
<p>You have been approached by a company that is studying human bahavior. Your task is to give them a webcam, that can detect the motion or any movement in front of it. This should return a graph, this graph should contain for how long the human/object was in front of the camera.</p>

<h2>Solution Logic : </h2>
<img src="Solution Logic.png" width="600" height="900">

<h2>Additional Python Libraries Required :</h2>
<ul>
  <li>OpenCV</li>
  
       pip install opencv-python
</ul>
<ul>
 <li>Pandas</li>
  
       pip install pandas
</ul>
<ul>
<li>Bokeh</li>
      
      pip install bokeh
</ul>
 
<h2>Analysis of all Windows :</h2>
  
After running the code there 4 new window will appear on screen.
<dl>
<dt>1. Gray Frame:</dt> 
<dd>In Gray frame the image is a bit blur and in grayscale we did so because, In gray pictures there is only one intensity value whereas in RGB(Red, Green and Blue) image thre are three intensity values. So it would be easy to calculate the intensity difference in grayscale.</dd>

<dt>2. Difference Frame:</dt> 
<dd>Difference frame shows the difference of intensities of first frame to the current frame.</dd>

<dt>3. Threshold Frame:</dt> 
<dd>If the intensity difference for a particular pixel is more than 30(in my code) then that pixel will be white and if the difference is less than 30 that pixel will be black.</dd>

<dt>4. Color Frame:</dt> 
<dd>In this frame you can see the color images in color frame along with green contour around the moving objects.</dd>

<h2>Time Record of Movements :</h2>
  
The Time_of_movements file will be stored in the folder where your code file is stored. This file will be in csv extension. In this file the start time of motion and the end time of motion will be recorded.

<h2>Plotting Time Intervals :</h2>

Time Intervals will be plotted using Bokeh Plot. Bokeh is an interactive visualization library that targets modern web browsers for presentation. Here, the time intervals are collected by the csv file and then plotted using Bokeh. The green color shows that an object was under motion, time is displayed in milisecond(ms).

<h2>Usage :</h2>

<b>The Repository contains 2 python files :</b>
<dl>
  <dt>motion_detector.py :</dt>
  <dd>It conatins the code for Motion Detection. By running this file you can detect the motion in front of webcam and can record the start and end time of motion.</dd>
  <dt>plotting.py :</dt>
  <dd>It makes use of Boken Library. By running this file you can plot the time intervals. This file imports the code of motion detection from motion_detector.py, so motion_detector.py needs to be in same directory.</dd>

# References:
<ul>
  <li>https://www.youtube.com/watch?v=-ZrDjwXZGxI</li>
</ul>
  
