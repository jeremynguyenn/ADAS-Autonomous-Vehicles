# ADAS_Collision_Avoidance
Advanced Driver Assistance System Using V2V Communication Based on STM32F103 and Raspberry Pi Microcontrollers.

# Introduction
Project includes some of advanced driver assistance system (ADAS) applications.
V2V technology used to communicate between vehicles.

# Why choose ADAS
- Reduced human error: by incorporating automation, ADAS aims to reduce human errors, a leading factor in road accidents, contribution to overall road safety..
- Safety enhancement: ADAS enhances vehicle safety through features like collision avoidance.
- Driver assistance: it provides real time assistance to drivers, improving overall driving experience by aiding in tasks like parking.
- Sensor integration: ADAS relies on various sensors such as Cameras, radar and Lidar to gather and process information for decision making.

# How ADAS work
![ADASwork](https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/ADAS_System.png)

# Porject flow chart
![ADASwork](https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/Picture5.png)

# V2V Communication
Vehicle-to-vehicle (V2V) communication’s ability to wirelessly exchange information about the speed and position of surrounding vehicles shows great promise in helping to avoid crashes, ease traffic congestion, and improve the environment.

Why V2V is important?
- V2V communication technology can increase the performance of vehicle safety systems and help save lives. 

- When one car brakes suddenly, for example, cars several yards behind the vehicle could get a safety warning before they get too close. 

# Linux with raspberry pi role in V2V
- The Blue Pill Interface with Raspberry Pi to Start the Measurements using UART. 
- Connect between Two Raspberry Pi by using MQTT. 
- send speed and direction from the first car to the second and create a graphical user interface (GUI) on a Raspberry Pi 3 B using both Qt or Tkinter.

# Connect between Two Raspberry Pi by using MQTT.
- ![image](https://github.com/user-attachments/assets/362d298e-b4a0-42ef-9845-ca9b6b1b2741)
- Flow chart
![flowchart](https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/Picture3.jpg)
- send speed and direction from the first car to the second and create a graphical user interface (GUI) on a Raspberry Pi 3 B using both Qt or Tkinter.
![flowchart](https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/Picture4.jpg)

# There are 3 main subsystems in this project 
## ADAPTIVE CRUISE CONTROL (ACC)
- Adaptive Cruise Control (ACC) is an advanced automotive technology designed to enhance driving safety and convenience. 
- The system precisely and efficiently controls the vehicle's speed, reducing driver fatigue and increasing comfort during long trips.
- ACC contributes to improved fuel efficiency by maintaining a steady speed and minimizing sudden acceleration and deceleration.
![image](https://github.com/user-attachments/assets/3344ef46-7497-4061-8235-f1488fcaed8a)
      How ACC work?
- The system utilizes a combination of sensors and communications between cars .
- ACC automatically adjusts the vehicle's speed to maintain a safe following distance from the car in front. When the vehicle approaches a slower-moving car, the system gradually reduces the speed to avoid the collision.
- Once the road ahead clears, the system accelerates the vehicle back to the preset speed chosen by the driver. 
![image](https://github.com/user-attachments/assets/7ee67ee7-3682-48e5-97f3-64290300ff9d)

      Flow chart main algorithm
![flowcharACC](https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/ADAPTIVE_CRUISE_CONTROL.png)

## AUTO EMERGENCY BRAKING SYSTEM (EBS)
- Nowadays, the number of accidents is so high and occurs everywhere, causing the worst damage, serious injuries, and death. These accidents can be caused due to the delay of the driver to hit the brakes.
- AEB is a safety system that can identify when a possible collision is about to occur and respond by autonomously activating the brakes to bring the vehicle to a stop to avoid the collision. 
![image](https://github.com/user-attachments/assets/17159e65-1423-487a-9d48-93587900d2d2)
      State of EBS or AEB:
Normal State
➢ Distance From Ultrasonic > MAXIMUM DISTANCE
Warning State
➢ MINIMUM DISTANCE <= Distance From Ultrasonic <= MAXIMUM DISTANCE
Auto Braking State
➢Distance From Ultrasonic < MINIMUM DISTANCE
![image](https://github.com/user-attachments/assets/7ca8d726-ed7b-4f80-9731-a23cdba23e51)

      Flow chart main algorithm
![imageAEB](https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/AEB.png)

## SELF-PARKING SYSTEM
- Most of the time people suffer from the problem of parking the car in the appropriate places due to high traffic demand, Following the rapid increase of car ownership, many cities are lacking car parking areas.
- This system simplifies the parking process, ensuring precise and safe maneuvering into parking spaces with minimal driver intervention.
- Ultrasonic sensors, scan continuously for available parking spaces and detect obstacles.
![image](https://github.com/user-attachments/assets/03fc127f-9dee-4668-b6db-9ff1d9ddc760)

        Flow chart main algorithm
![flowchartselfdriving](https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/SELF_PARKING_SYSTEM.png)

# DEMO for each subsystems
- DAPTIVE_CRUISE_CONTROL:

https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/video1.mp4

- AEB:

https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/video2.mp4

-Self-driving:

https://github.com/jeremynguyenn/Autonomous-Vehicles/blob/main/ADAS_Collision_Avoidance/pic/video3.mp4
