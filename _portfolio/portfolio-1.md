---
title: "Quadcopter"
excerpt: "Full design and development of quadcopter 1<br/><img src='/images/quadcopter.jpg'>"
collection: portfolio
---

I built this quadcopter from scratch designing the frame in solidworks and 3D printing. I bought all of the electronics and the propellers for this build:

- 6-DOF IMU containing an accelerometer and a gyroscope (MPU-6050)
- 4 in 1 ESC
- Arduino as my flight controller
- 2300 KV motors
- Radio transmitter/receiver

The code I used for the Arduino was taken from [https://github.com/lobodol/drone-flight-controller](https://github.com/lobodol/drone-flight-controller) and edited as needed. There were two separate scripts I used, one for calibrating the ESC and the other was the flight controller. The major tasks of the flight controller was filtering the IMU data and creating roll, pitch, and yaw commands from the radio transmitter. I used a PID controller for roll, pitch and yaw to accomplish this. I used this [publication](https://ieeexplore.ieee.org/document/7813499) to help my understanding with the controller and the physical modeling.

One challenge I ran into was I initially tried to 3D print the propellers but figured out very quickly that they created too much drag and ended up buying propellers. 

This is an item in your portfolio. It can be have images or nice text. If you name the file .md, it will be parsed as markdown. If you name the file .html, it will be parsed as HTML. 
