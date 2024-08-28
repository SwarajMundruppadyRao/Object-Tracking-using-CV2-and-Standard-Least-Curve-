# Object Tracking Using CV2

# Description 

This repository contains code for tracking an object's trajectory and plotting the path of its center using Standard Least Squares Curve Fitting. This project was completed as part of ENPM673 Project I.

# Dependencies 

1. numpy
2. cv2
3. matplotlib
   
## Installation

To set up the required Python packages, run the following command:

```bash
sudo apt-get install python3-numpy python3-opencv python3-matplotlib
```

# Pipeline

1. Read the Video: Load the video file for processing.

   ![image](https://github.com/user-attachments/assets/06bfcea3-22f0-468b-b174-e73073fbda48)

2. Extract Black Pixel Coordinates: Identify and extract coordinates of black pixels in each frame. This approach is used because the object of interest is a black bag.
   
3. Calculate Centroid: Compute the centroid of the black pixels in each frame to determine the object's center.
   ![image](https://github.com/user-attachments/assets/58563200-e79c-4673-ac64-38bb1e95129a)

4. Plot the Trajectory: Use the collection of centroids to plot the object's path, applying Standard Least Squares Curve Fitting to smooth and analyze the trajectory.
![image](https://github.com/user-attachments/assets/9db3d7bc-e943-47d2-a41f-f917603bf03f)

