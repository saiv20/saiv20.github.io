---
layout: page
title: Multirobot navigation in ROS and Gazebo
description:
img: assets/img/S1.png
importance: 5
category: work
giscus_comments: false
---
<b>Code:</b> [![GitHub Badge](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=fff&style=flat)](https://github.com/saiv20/multirobot_tb)<br>

This ROS package implements navigation for multiple robots autonomously. Initially, Simultaneous Localization and Mapping (SLAM) gmapping is used to map the unknown environment. Once the environment is mapped and the map is generated, multiple robots are navigated autonomously on the map using the ROS Navigation Stack.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/S1.png" title="Gazebo_Image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/S2.png" title="Gazebo_Image2" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

For further usage instructions, visit the github page.