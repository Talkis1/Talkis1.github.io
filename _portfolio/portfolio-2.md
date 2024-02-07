---
title: "Quadcopter"
excerpt: "<br/><img src='/images/quadcopter.jpg' width='500'>"
collection: portfolio
---

I built this quadcopter from scratch designing the frame in solidworks and 3D printing. I bought all of the electronics and the propellers for this build:

- 6-DOF IMU containing an accelerometer and a gyroscope (MPU-6050)
- 4 in 1 ESC
- Arduino as my flight controller
- 2300 KV motors
- Radio transmitter/receiver

The code I used for the Arduino was taken from [https://github.com/lobodol/drone-flight-controller](https://github.com/lobodol/drone-flight-controller) and edited as needed. There were two separate scripts I used, one for calibrating the ESC and the other was the flight controller. The major tasks of the flight controller was filtering the IMU data and creating roll, pitch, and yaw commands from the radio transmitter. I used a PID controller for roll, pitch and yaw to accomplish this. I used this [publication](https://ieeexplore.ieee.org/document/7813499) to help my understanding with the controller and the physical modeling.

Here is a video of testing the quadcopter:
<iframe width="560" height="315" src="https://www.youtube.com/embed/IQm0eE9rv6U" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
