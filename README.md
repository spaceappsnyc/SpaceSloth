# SpaceSloth
Welcome to the SpaceSloth Helmet!

As a team of 7 people at the Space Apps NYC Hackathon 2015 we created a sensing helmet that would record and process measurements from and through:
* 5 IR proximity sensors (4-30 cm range) 
* 1 LIDAR Lite (Range: 0-40m Laser Emitter, Accuracy: +/- 0.025m) 
* 1 Logitech camera 
* 1 Arduino Uno 
* 1 Intel Edison Board 
* 1 Moto X Smartphone 
* 1 LG Smart Watch 

We implemented a working version of:
* Reading the measurements of three IR Sensors through the Intel Edison Board and visualizing them on a server 
* Reading the measurements of the LIDAR Sensor on an Arduino Uno and sending those measurements to the Intel Edison Board via Serial RX & TX pins 
* Applying color object detection to the output of the camera and return the position and size of the object within each picture frame (used to track the Astronaut Sloth who was tagged with a piece of red cloth) 
* Vibrated the LG Smart Watch through the Moto X when an obstacle came closer

