# Adaptive-Intelligent-Transportation-System
Adaptive intelligent transportation system
Hello, I’m Cheng, and today I am going to guide my FPGA project on board DE1-SOC, and my project name is ‘Adaptive intelligent transportation system’. The purpose of the project is dealing with the various road conditions, and aim to reduce traffic jam by adaptive changing the frequency of traffic lights.
  
  The system is mainly divided into five parts, respectively are the car following distance measurement, manual control through mode switches, LEDR warning system, automatically adapt controller, and manager system.
  
  Firstly, as you can see, we use the HC-SR04 as the sensor to measure the distance as the car following distance, and the distance is shown by the digital segment on the right side. After this, to remind the driver driving safely, we bring in a warning light, the closer two cars are, the faster the warning light flashes.
 
 Except this, the two left switches are controlling the road situation, such as morning rush/evening rush or normal time, or low traffic. Each road situation turns to different basic time for traffic light. Furthermore, the time for green and red lights are also changing with the car following distance, because the lower the average distance, the more it indicates that the road is congested. What is more? We also implement a manager system to manually control frequency of the lights. When we enter the correct cypher, the LEDR7 will be light on to shows that cypher correct, and when we push KEY3 or KEY1, the lasting time for red and green light will increase or decrease. 
  
  So, our project can adaptively change the traffic light due to the current road situation.
