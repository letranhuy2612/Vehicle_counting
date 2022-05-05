# Vehicle_counting

## Overview
This project aims to count every vehicle (motorcycle,bus,car,truck) detected in the input video using YOLOv3 object-detection and centroid tracker algorithm.

## Working
![Screenshot 2022-05-05 124029](https://user-images.githubusercontent.com/85574548/166873146-b6b476b2-0ede-4886-876a-ef98ea06b134.png)

## Implementation details
The detections are performed on each frame by using YOLOv3 object detection algorithm and displayed on the screen with bounding boxes.

The center of each box is taken as a reference point (denoted by a red dot when performing the detections) when track the vehicles.

Calculates the difference between two center points of an object in the current frame vs the previous frame, and if the distance is less than the threshold distance then it confirms that the object is the same object of the previous frame.


