# Wireless Motor PWM Control System

## Overview
This project is a wireless motor speed control system developed for an Embedded Systems course. The system allows a user to send speed commands from a smartphone through Bluetooth. The MSP430FR2355 microcontroller receives the command through UART and generates a PWM signal to control a 12V DC motor through an L298N motor driver.

An I2C LCD displays the current motor speed percentage in real time.

This project helped me practice embedded systems, PWM motor control, UART communication, Bluetooth integration, hardware wiring, and real-time output display.

## Key Skills
- Embedded Systems
- C Programming
- MSP430FR2355 Microcontroller
- UART Communication
- PWM Motor Control
- I2C LCD Display
- HM-11 Bluetooth Module
- L298N Motor Driver
- DC Motor Control
- Hardware Debugging

## Hardware Used
- MSP430FR2355 microcontroller
- HM-11 Bluetooth module
- L298N motor driver
- 12V DC motor
- 16x2 I2C LCD
- External 12V power supply
- Breadboard and jumper wires

## System Workflow
1. The user enters a speed command on a smartphone.
2. The HM-11 Bluetooth module receives the command.
3. The Bluetooth module sends the command to the MSP430FR2355 through UART.
4. The MSP430 processes the input and updates the PWM duty cycle.
5. The L298N motor driver controls the speed of the 12V DC motor.
6. The I2C LCD displays the selected motor speed percentage.

## System Block Diagram

````markdown
## System Block Diagram

```text
Smartphone
   ↓ Bluetooth
HM-11 Bluetooth Module
   ↓ UART
MSP430FR2355 Microcontroller
   ↓ PWM Signal
L298N Motor Driver
   ↓ Motor Power
12V DC Motor

MSP430FR2355
   ↓ I2C
16x2 LCD Display

## How PWM Controls Motor Speed

PWM stands for Pulse Width Modulation. It controls motor speed by switching the signal ON and OFF very quickly. The duty cycle determines how much power is delivered to the motor.

```text
25% duty cycle  → Low speed
50% duty cycle  → Medium speed
75% duty cycle  → High speed
100% duty cycle → Full speed
```

A higher duty cycle means the motor receives more average power, so it spins faster.

## Why a Motor Driver Was Used

The microcontroller cannot directly power a 12V DC motor because the motor requires more voltage and current than the MSP430 pins can safely provide.

The L298N motor driver acts as an interface between the low-power control signal from the microcontroller and the higher-power motor circuit. This protects the microcontroller and allows the motor to operate using an external 12V supply.

## Main Features

- Wireless speed control using Bluetooth
- UART communication between Bluetooth module and microcontroller
- PWM-based DC motor speed control
- Real-time speed percentage display on I2C LCD
- External motor power through L298N driver
- Hands-on embedded hardware integration

## Challenges

One challenge was making sure the motor received enough power without damaging the microcontroller. The motor needed a separate 12V supply, while the MSP430 only handled the control signal.

Another challenge was correctly receiving Bluetooth commands through UART and converting those commands into different PWM duty cycles.

A third challenge was integrating the I2C LCD so the system could display the selected motor speed clearly in real time.

## Result

The final system successfully controlled the speed of a 12V DC motor wirelessly using Bluetooth commands. The MSP430FR2355 generated PWM signals based on the received command, the L298N motor driver controlled the motor output, and the I2C LCD displayed the selected speed percentage.

## What I Learned

Through this project, I learned how embedded software and hardware work together in a real system. I gained hands-on experience with UART communication, PWM signal generation, motor driver circuits, Bluetooth modules, and LCD display integration.

This project also helped me understand the importance of power management, debugging, and testing when working with hardware systems.

## Future Improvements

In the future, I would improve this project by:

- Adding motor speed feedback using a sensor
- Implementing closed-loop speed control
- Adding reverse direction control
- Creating a PCB version of the circuit
- Improving Bluetooth range and reliability
- Adding a mobile app interface with buttons or sliders

## Project Status

Completed as a working prototype for embedded systems and portfolio development.
