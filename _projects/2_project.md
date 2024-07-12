---
layout: page
title: Visual SLAM using ORBSLAM3 and Dead Reckoning
description: 
img: assets/img/3.jpg
importance: 2
category: work
giscus_comments: false
---

This project involved the acquisition and analysis of real-time odometry and camera data from Northeastern University's autonomous car, NUANCE. The primary objective was to implement Visual SLAM using ORBSLAM3 and perform dead reckoning on the collected rosbag. The magnetometer was calibrated and the data was fused with gyroscope data using a complementary filter and Extended Kalman Filter (EKF) to provide a more accurate estimate of the orientation. This filtered yaw and position estimate was used for dead reckoning. 

The magnetometer calibration is shown below. We calibrate for both soft iron and hard iron distortions.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Entire_Curve.jpg" title="Entire_Curve" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The yaw is shown below.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/yawvtime.jpg" title="Yaw" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The GPS and IMU velocity after bias is shown below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gpsvel.jpg" title="GPSVel" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Now, lets look at a simple example of ORBSLAM3. For that, we took a video around Northeastern. We made a loop around the buildings. For this experiment, we just used camera without any inertial sensors. The output of ORBSLAM3 is shown below.

<iframe src="https://drive.google.com/file/d/1OsWBAp6yXJOysPZtvN2bQZYKntURJpU_/preview" width="640" height="480" allow="autoplay"></iframe>

Once we complete the loop, we can see loop closure in ORBSLAM3 as well.

Now, lets apply the same ORBSLAM3 to the data we obtained from Northeastern University’s autonomous car (NUANCE).

<iframe src="https://drive.google.com/file/d/1zw6G9D8uxGTWCSkEFgtcv88KDkFJuE3X/preview" width="640" height="480" allow="autoplay"></iframe>