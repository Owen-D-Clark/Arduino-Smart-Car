# Arduino-Smart-Car
This project implements a robot car controlled using either MPU6050 accelerometer/gyroscope input or analog joystick input, programmed in Arduino C/C++. The software reads motion data via I2C using the Wire and MPU6050 libraries, then maps raw accelerometer values into a normalized 0–255 control range. These values are processed using calibrated threshold logic to determine directional movement (forward, backward, left, right, stop).

The control system uses structured data handling and conditional logic to convert sensor input into digital motor control signals, driving an H-bridge motor driver through GPIO pins. The same control architecture was modularly adapted to support joystick input using analogRead(), demonstrating flexibility in input abstraction.
