## Perception

To provide perception capabilities to your mobile robot you need a sensor like a RGB or RGB-D camera as hardware and software like 
[OpenCV](https://opencv.org/) or [PCL](https://pointclouds.org/).


!!! quote
    OpenCV (Open Source Computer Vision Library) is a library of programming functions mainly aimed at real-time computer vision. 
    Originally developed by Intel, it was later supported by Willow Garage then Itseez (which was later acquired by Intel). 
    The library is cross-platform and free for use under the open-source Apache 2 License. 
    Starting with 2011, OpenCV features GPU acceleration for real-time operations.
    
    
!!! quote
    The Point Cloud Library (PCL) is a standalone, large scale, open project for 2D/3D image and point cloud processing. 
    PCL is released under the terms of the BSD license, and thus free for commercial and research use.


When working with OpenCV and ROS we have to install required dependency using `ros-noetic-vision-opencv`. This will install additional dependencies like OpenCV (`libopencv-dv`) and `ros-noetic-cv-bridge`. There is no need to install OpenCV from source or the Ubuntu binaries (deb package).

If you want to use OpenCV without ROS you should consider installing it from [source using CMake](https://docs.opencv.org/master/d7/d9f/tutorial_linux_install.html). 
This will allow you to configure what features should be installed, e.g., example code.
Otherwise you can install a pre compiled binary `libopencv-dev`.
{: .notice }

Similar to work with PCL and ROS you need to install the dependency `ros-noetic-perception-pcl`, which is the interface between ROS and PCL.


To work with PCL without ROS you should consider installing it from [source using CMake](https://pointclouds.org/documentation/tutorials/building_pcl.html). 
This will allow you to configure what features should be installed, e.g., example code.
Otherwise you can install a pre compiled binary `libpcl-dev`.
{: .notice }

[`perception_pcl`](https://wiki.ros.org/perception_pcl) is a meta package for PCL (Point Cloud Library) ROS interface stack. 
PCL-ROS is the preferred bridge for 3D applications involving n-D Point Clouds and 3D geometry processing in ROS.
