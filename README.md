# 8240-Autonomous-Navigation-on-Road-

Academic Project at Clemson University - International Centre for Automotive Research 
### -----Can't share code here due to academic restrictions-----


## Problem Statement:

The project's problem statement includes completing 4 different tasks and 
integrating it. The four tasks are as follows:

### 1. Autonomous Lane Keeping:
Autonomously track the lane clockwise using a camera and a laptop as fast as 
possible.
### 2. Recognize road signs:
Autonomously recognize a stop sign and a school zone using a second camera and a 
laptop.
### 3. Communications:
Send the road sign information from the second laptop to first laptop through Wi-Fi 
communications.
### 4. Vehicle Controls: 
Stop the vehicle at the stop sign for 2 seconds and then run at high speed; Reduce 
the speed by half at the school zone sign.

## Technical Approach:

### 1. Camera Calibration

Camera calibrartion using checkerboard pattern

<img width="258" alt="image" src="https://user-images.githubusercontent.com/79803663/167763644-ec074cb4-976f-43b3-9881-740ca0872b9f.png">

Parameters found after camera calibration

<img width="386" alt="image" src="https://user-images.githubusercontent.com/79803663/167763771-ef7b56d9-4622-4f09-948e-c0f57ed45add.png">

### 2. Detection of Track

Implementation of color masking

![image](https://user-images.githubusercontent.com/79803663/167764006-54be2cf1-2dbf-4f99-ac75-f948813b9e5c.png)

Following the track

![image](https://user-images.githubusercontent.com/79803663/167764068-9d5ba321-e3cb-466d-8ffd-55d32267a75d.png)

Averaging method

![image](https://user-images.githubusercontent.com/79803663/167764107-ddf4c963-48bc-48d0-bb6a-a18027689db1.png)

### 3. Controller

Steering angle based on averaging metod
![image](https://user-images.githubusercontent.com/79803663/167764158-16468f4e-6d50-4133-9447-ba4c26bac108.png)

### 4. Stop sign detection

R-CNN Transfer Learning using CIFAR10Net was used for the implementation of stop sign detection

![image](https://user-images.githubusercontent.com/79803663/167764520-2a7b4cd5-337d-412e-96e5-2a375ade7ef5.png)


![image](https://user-images.githubusercontent.com/79803663/167764533-2eeea79a-e29f-4c72-9834-f23115148a4f.png)

### 5. Communication

Communication between laptop is done using UDP protocol.

![image](https://user-images.githubusercontent.com/79803663/167764576-38d697ea-c181-438e-9a1b-4e57a9b38015.png)


## Vehicle Testing on Track:



https://user-images.githubusercontent.com/79803663/167766219-d559dd13-69b9-4a11-81e3-32819af80b8f.mp4

