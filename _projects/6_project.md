---
layout: page
title: Pedestrian Detection
description:
img: assets/img/ped_det.jpg
importance: 6
category: work
giscus_comments: false
---
<p align="justify">
In this project, we compare three famous object detection algorithms - Faster RCNN, YOLOv8, and DETR(DEtection TRansformers) for pedestrian detection.
For this purpose, we captured a video with pedestrians and vehicles at a busy intersection.
</p>

The video below shows the output for Faster RCNN.
<iframe src="https://drive.google.com/file/d/1fdXFgAoFE6EMyNunAjaUFeHimdrrNWnF/preview" width="640" height="480" allow="autoplay"></iframe>

The video below shows the output for YOLOv8.
<iframe src="https://drive.google.com/file/d/1o0gbIpjiOkxnSsvvEE2AId1QpUHA1eHR/preview" width="640" height="480" allow="autoplay"></iframe>

The video below shows the output for DETR.
<iframe src="https://drive.google.com/file/d/1cVl4JQHOyiMgbh2hzBGCZYBa41CzZYHm/preview" width="640" height="480" allow="autoplay"></iframe>

<p align="justify">
From the comparison, we observe that DETR excels in accurately detecting pedestrians,
including those located far away. While Faster R-CNN performs well overall, it can sometimes
misclassify objects such as bikes and parking meters as pedestrians. YOLOv8, on the other
hand, shows fewer misclassifications compared to Faster R-CNN but fails to detect a pedestrian
crossing the street. Despite these accuracy differences, YOLOv8 stands out for its real-time
performance capabilities, whereas Faster R-CNN and DETR require more time for inference.
</p>