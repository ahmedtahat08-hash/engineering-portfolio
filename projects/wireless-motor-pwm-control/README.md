# Wireless Motor PWM Control System

## Overview

This project is a wireless motor speed control system developed for an Embedded Systems course. The system allows a user to send speed commands from a smartphone through Bluetooth. The MSP430FR2355 microcontroller receives the command through UART and generates a PWM signal to control a 12V DC motor through an L298N motor driver.

An I2C LCD displays the current motor speed percentage in real time.

## Key Skills

Embedded Systems, C Programming, MSP430FR2355, UART, PWM, I2C LCD, HM-11 Bluetooth, L298N Motor Driver, Motor Control

## Hardware Used

- MSP430FR2355 microcontroller
- HM-11 Bluetooth module
- L298N motor driver
- 12V DC motor
- 16x2 I2C LCD
- External 12V power supply

## System Workflow

1. User enters a speed command on the smartphone.
2. Bluetooth sends the command to the HM-11 module.
3. HM-11 forwards the data to the MSP430 through UART.
4. MSP430 processes the input and updates the PWM duty cycle.
5. L298N motor driver changes the 12V DC motor speed.
6. I2C LCD displays the selected speed percentage.

## Project Highlights

- Designed and tested a wireless motor speed control system using MSP430FR2355, HM-11 Bluetooth, L298N motor driver, UART, PWM, and a 12V DC motor.
- Programmed C-based motor control logic to receive smartphone speed commands from 0% to 100% and adjust motor speed in real time.
- Integrated an I2C LCD display to show live motor speed feedback.
- Tested the system with multiple speed inputs and confirmed stable Bluetooth communication and proportional motor response.

## Resume Bullets

- Designed and tested a wireless motor speed control system using MSP430FR2355, HM-11 Bluetooth, L298N motor driver, UART, PWM, and a 12V DC motor.
- Programmed C-based motor control logic to receive smartphone speed commands from 0% to 100% and display real-time feedback using an I2C LCD.

## Suggested Images to Add Later

- Final hardware setup photo
- Wiring diagram
- Block diagram
- LCD display photo
- Smartphone app screenshot
- Demo video link
