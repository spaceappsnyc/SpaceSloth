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

VISUALIZATION:

We made a very basic GUI formed of three equal width divs. Each div was respectively linked to the data transmitted from the three IR proximity sensors that was placed on the left, center and right side of the helmet and had ten greyscale color states that ranged from #000000(black) to #999999 (light gray). The closer the wall is to the sensor, the lighter the color of the div gets. With this simple visual aid, one could navigate through walls and mazes while wearing the helmet by walking slowly towards the darker shade. 

Our future plans for the GUI involved adding two more divs to the screen and dividing the center div into another two divs stacked on top of the other. The top div would be linked to the LIDAR that's attached to the front of the helmet and contain roughly hundred color states that range from black to light blue. The bottom would be linked to another IR sensor in the back of the helmet and would behave as the other greyscale divs. 
In the future version of the GUI, the object location data detected from the camera would be overlayed on top of all the divs and be visualized by a red dot with a scalable size depending on its distance to the helmet.
