# line-follower-robot
# Line-Following Robot with Obstacle Detection

## Project Overview
This project is a microcontroller-based robot using **Arduino**, **IR sensors**, and **PWM motor control** to follow a line and avoid obstacles. The robot can autonomously track a path using two IR sensors and stops when detecting obstacles with an ultrasonic sensor. Messages are displayed on an LCD, and an LED signals obstacle detection.

---

## Features
- Line-following using two IR sensors (`RIR` and `LIR`)  
- Obstacle detection using an ultrasonic sensor (`TP` and `EP`)  
- LED and LCD feedback for obstacle alerts  
- Motor control via PWM for left and right motors  
- Simple if-else logic for line-following behavior  

---

## Hardware Components
- Arduino Uno (or compatible microcontroller)  
- IR sensor array (2 sensors)  
- Ultrasonic sensor (HC-SR04 or equivalent)  
- DC motors with driver  
- LEDs for status indicators  
- LCD display (I2C)  
- Chassis, wheels, battery pack  

---

## Software & Tools
- Arduino IDE  
- C++ programming  
- SoftwareSerial library for Bluetooth  
- LiquidCrystal_I2C library for LCD display  

---

## How It Works
1. **Line Following:** The IR sensors detect the line and adjust motor outputs via if-else logic.  
2. **Obstacle Detection:** The ultrasonic sensor measures distance. If an obstacle is detected (<14 cm), the robot stops and displays a warning on the LCD while blinking the internal LED.  
3. **Motor Control:** Motor speeds are controlled using PWM signals to move forward, stop, or turn based on sensor input.  

---

## Notes
- PID control is **not implemented**; the robot uses simple conditional logic for steering.  
- Speed measurements should be verified physically if claiming specific m/s performance.  

---

## Author
**Iyad Shomar**  
