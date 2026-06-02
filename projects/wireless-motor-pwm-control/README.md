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
