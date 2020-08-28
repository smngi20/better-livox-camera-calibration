# Better Livox Camera Calibration 


__READ HERE FOR MORE INFO__ : [ORIGINAL SOURCE REPOSITORY](https://github.com/Livox-SDK/livox_camera_lidar_calibration) 


## MAJOR CHANGES 
### Added Better Intrinsic Camera Calibration TOOL 
- Use __newCalibrate.py__ for calculating intrinsic parameters and paste into the ROS WORKFLOW 
### Added New ViewPorts ProjectCloud.launch
- The basic COLOR based projection of point clouds on the image was not clear enough for use so we build a scaled greyscale projection. 
- After Calibration Run ProjectCloud.launch from the ROS launch files. 
- see: __getColor2__ function in the src cpp 
### Made the Output Pipline Independent of ROSBAG 
- Made an input parser for PCD files using pcl_ros instead of the premade ROSBAG method as PCD's are more flexible. 
- Location for PCD read is mentioned in the respective ROS file. 


_ALL CHANGES ARE SOMEWHAT EDITABLE AS MOST ORIGINAL CODE IS COMMENTED AND MY ADDITIONS ADDED AS OPTIONS_
