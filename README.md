# Arduino L298N DC Motor Control

## Overview

This project explores DC motor control using an Arduino Uno and an L298N dual H-bridge motor driver.

The objective was to understand how microcontrollers interface with DC motors, how an H-bridge controls motor direction, and how PWM signals can be used to regulate motor speed.

The setup uses two geared DC motors connected to an L298N motor driver, controlled through an Arduino Uno.

## Project Objectives

- Understand the working principle of an H-bridge motor driver.
- Interface an L298N motor driver with an Arduino Uno.
- Control the direction of rotation of two DC motors.
- Explore PWM-based motor speed control.
- Understand GPIO configuration and digital output control.
- Gain practical experience with embedded hardware interfacing.

## Hardware Components

| Component | Purpose |
|---|---|
| Arduino Uno | Main microcontroller |
| L298N | Dual H-bridge motor driver |
| 2 × Geared DC motors | Vehicle movement |
| Wheels and chassis | Mechanical assembly |
| Battery supply | Motor power |
| Breadboard and jumper wires | Electrical connections |

## Working Principle

The Arduino Uno generates digital control signals that are received by the L298N motor driver.

The L298N uses an H-bridge configuration to control the polarity of the voltage supplied to each motor, allowing forward and reverse rotation.

The motor enable inputs can receive PWM signals from the Arduino to regulate motor speed.

By independently controlling the two motors, the vehicle can perform different movements:

- Forward: Both motors rotate in the forward direction.
- Reverse: Both motors rotate in the reverse direction.
- Left turn: The motors rotate in opposite directions or at different speeds.
- Right turn: The motor directions or speeds are adjusted accordingly.
- Stop: Motor drive is disabled.

## System Connections

The following is the intended Arduino-to-L298N pin mapping. Update it if your actual wiring differs.

| Arduino Uno | L298N |
|---|---|
| D5 (PWM) | ENA |
| D6 (PWM) | ENB |
| D8 | IN1 |
| D9 | IN2 |
| D10 | IN3 |
| D11 | IN4 |
| GND | GND |

Motor connections:

- Left motor: OUT1 and OUT2
- Right motor: OUT3 and OUT4

## Software

- Arduino IDE

## Learning Outcomes

Through this project, I gained practical exposure to:

- Arduino GPIO programming.
- PWM-based motor speed control.
- H-bridge motor driver operation.
- DC motor direction control.
- Microcontroller-to-hardware interfacing.
- Basic electronics assembly and troubleshooting.


## Future Improvements

- Integrate an HC-05 Bluetooth module for smartphone-based control.
- Interface an ultrasonic sensor for obstacle detection.
- Implement IR sensor-based line following.
- Add independent motor speed adjustment and smoother turning.
- Explore closed-loop motor speed control using encoders.

## Author

Rahul Santhosh

Embedded Systems | Arduino | C Programming

