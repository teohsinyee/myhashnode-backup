# Robotics Practice (Case study Part 2)

Round 1: Quick Recall (Do not look at the lecture notes)  
Round 2: Fill up the gap by screening through the lecture notes

Essay Question 1 (100 marks):

1) Explain the basic structure and components of a wheeled robot (20 marks).
    
      
    <mark>My answer:</mark>
    
    It has wheels to move around. Sensors are used to avoid obstacles. Battery to supply power. Motor to support the engine.
    
      
    <mark>Chat-GPT:</mark>
    
    A wheeled robot typically has the following components:
    
    * Chassis: The main body of the robot that holds all the other components together.
        
    * Wheels: The primary means of locomotion for the robot.
        
    * Motors: To drive the wheels and control the robot's movement.
        
    * Battery: To power the motors and other components of the robot.
        
    * Sensors: To perceive the environment and help the robot make decisions.
        
    * Microcontroller: To process sensor data and control the motors.
        
    * Power management system: To regulate the power supplied by the battery to the various components.
        
2) Describe the various types of sensors used in robots, including their function and applications (30 marks).  
      
    <mark>My answer:</mark>
    
    Infrared sensor detects object that is far away from it, it is widely used in vacuum robot. Ultrasound sensor is similar to infrared but able to detect longer distance than infrared. LIDAR also similar, but detect the furthest. Light sensor detects light. Touch sensor detects object, normally used in obstacle avoidance.
    
      
    <mark>Chat-GPT:</mark>
    
    There are several types of sensors that are commonly used in robots, including:
    
    * Infrared sensors: Used to detect objects at a distance, often used in vacuum robots.
        
    * Ultrasonic sensors: Similar to infrared sensors but able to detect objects at a longer distance.
        
    * LIDAR sensors: Similar to ultrasonic sensors but can detect objects at even greater distances.
        
    * Light sensors: Used to detect changes in light levels, often used for light following or line following applications.
        
    * Touch sensors: Used to detect physical contact, often used in obstacle avoidance.
        
    * Cameras: Used to capture visual data, often used for object recognition and navigation.
        
3) Discuss the challenges and techniques for robot navigation, including dead reckoning and SLAM (30 marks).  
      
    <mark>My answer:</mark>
    
    Robot navigation is challenging because to navigate without collision, we need to install good sensors on the robot, which it required high cost. To move fast, an efficient algorithm is in dire to plan the path, so the robot can reach destination quickly. Techniques for navigation are divided into dead reckoning and SLAM. Dead reckoning is less costly because the robot will navigate based on the map the planned beforehand. SLAM navigates based on the real-time scenario. The navigation route will be changed halfway based on the needs.
    
      
    <mark>Chat-GPT:</mark>
    
    Navigating a robot can be challenging because it requires the robot to make decisions about its movement while avoiding obstacles and reaching its destination. Some of the main challenges in robot navigation include:
    
    * Cost: High-quality sensors and processing power can be expensive.
        
    * Complexity: Navigating a robot requires a lot of computing power and sophisticated algorithms.
        
    * Accuracy: The robot needs to have a high level of accuracy in order to avoid collisions and reach its destination.
        
    
    Two common techniques for robot navigation are dead reckoning and SLAM (Simultaneous Localization and Mapping). Dead reckoning is a method of navigation that uses the robot's movements to estimate its position and orientation. SLAM, on the other hand, involves creating a map of the environment as the robot moves through it, and using this map to localize the robot in real-time.
    
4) Outline the steps involved in the localization process, including the use of Monte Carlo localization (20 marks).  
      
    <mark>My answer:</mark>
    
    Localization means the location of robot. To know robot location, we can install GPS on it.  
    
    <mark>Chat-GPT:</mark>
    
    Localization refers to the process of determining the position and orientation of a robot in its environment. Some of the steps involved in the localization process include:
    
    * Collecting sensor data: The robot needs to gather data from its sensors, such as cameras, LIDAR, and ultrasonic sensors, in order to make a map of its environment.
        
    * Processing sensor data: The robot needs to process the sensor data and use it to create a map of its environment.
        
    * Monte Carlo localization: This is a specific localization algorithm that uses a probabilistic approach to estimate the robot's position and orientation. It involves generating many possible hypotheses about the robot's location and updating these hypotheses based on new sensor data.