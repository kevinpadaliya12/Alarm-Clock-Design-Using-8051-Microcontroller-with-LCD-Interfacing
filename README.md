# Alarm-Clock-Design-Using-8051-Microcontroller-with-LCD-Interfacing

This repository contains the firmware and design files for a fully functional Digital Alarm Clock built using the classic 8051 (AT89C51) microcontroller. This project is an excellent demonstration of embedded systems fundamentals, including hardware interfacing, real-time programming, and peripheral management.

Features

Real-Time Clock: Displays the current time in HH:MM:SS format.
Alarm Functionality: Allows the user to set a specific alarm time.
User-Friendly Interface: A 4x3 matrix keypad for setting the current time and alarm time.
Clear Visual Display: A 16x2 character LCD screen provides clear prompts and time display.
Audible Alert: An onboard buzzer activates when the current time matches the set alarm time.

Hardware Components

Microcontroller: AT89C51 (or any standard 8051 variant)
Display: 16x2 Character LCD Display
Iput: 4x3 Matrix Keypad
Alert: 5V Piezo Buzzer
Oscillator: 11.0592 MHz Crystal Oscillator
Capacitors: 2 x 22pF (for the crystal)
Resistors: As required for pull-ups or current limiting.
Power Supply: 5V DC Power Source
Prototyping Board: Breadboard or a custom PCB

Software & Tools

IDE: Keil µVision IDE
Compiler: C51 Compiler
Programming Language: Embedded C
Simulation (Optional): Proteus Design Suite for circuit simulation.

 How It Works
 
The system is built around the 8051 microcontroller, which orchestrates all operations.
Initialization: On power-up, the microcontroller initializes the LCD and all I/O ports.
Set Time: The user is prompted via the LCD to enter the current time (hours and minutes) using the matrix keypad.
Timekeeping: The core of the clock is a precise 1-second delay generated using the 8051's internal hardware timer (Timer 0). The firmware increments a seconds counter after each delay, handling the rollover to minutes and hours.
Set Alarm: The user can press a dedicated key to enter the alarm-setting mode, inputting the desired alarm time.
Alarm Check: In its main loop, the firmware continuously compares the current time with the stored alarm time
Trigger Buzzer: If the times match, the microcontroller sends a signal to activate the buzzer.

circut diagram
<img width="940" height="613" alt="image" src="https://github.com/user-attachments/assets/a0975cd5-54a5-45e0-807e-5bc3305677cf" />

