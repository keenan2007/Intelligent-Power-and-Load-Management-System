# Intelligent-Power-and-Load-Management-System

## Overview
This project is an Arduino-based power load management system designed to simulate how electrical loads can be monitored and controlled based on changing demand.

A potentiometer is used to simulate variations in system demand. The Arduino reads this input and responds by activating different LED indicators and controlling a DC motor through a transistor.

The project was created to develop my understanding of electrical systems, load monitoring, circuit design, and hardware control.

## How It Works
The potentiometer provides an analog input to the Arduino representing the current system demand.

The Arduino continuously reads this value and determines the appropriate system response.

Depending on the demand level:
- LEDs indicate different operating conditions
- The DC motor acts as a controllable electrical load
- The Arduino determines when different outputs should be activated

The motor is controlled using an NPN transistor rather than being powered directly from an Arduino output pin.

A diode is connected across the motor to protect the circuit from voltage spikes produced when the motor is switched off.

## Components
- Arduino Uno
- Potentiometer
- DC motor
- NPN transistor
- Flyback diode
- Red, green, and blue LEDs
- Resistors
- Breadboard
- Jumper wires

## Control Logic
The Arduino reads the potentiometer using an analog input.

The input value is divided into different demand ranges, and the system activates the appropriate LEDs and motor behavior based on the measured value.

This allows the system to simulate basic automatic load management.

## Circuit Design
The circuit includes:
- Analog input from the potentiometer
- LED status indicators
- Transistor-based motor switching
- Diode protection for the motor
- Arduino-based control logic

## Design Challenges
Several issues occurred during development and required troubleshooting.

One early problem was incorrect LED and resistor placement on the breadboard, which prevented one of the LEDs from operating correctly.

Another challenge occurred when adding the DC motor. The motor initially did not run because the transistor was wired incorrectly. After reviewing the collector and emitter connections and correcting the wiring, the motor operated successfully.

These problems helped reinforce the importance of checking circuit connections systematically and understanding the function of each component.

## What I Learned
This project helped me develop experience with:
- Arduino analog inputs
- Electrical load control
- Potentiometers and sensor-style inputs
- Transistor switching
- DC motor control
- Flyback diode protection
- Breadboard circuit design
- Hardware troubleshooting
- Basic automated control logic

  ## Design Link:
  https://www.tinkercad.com/things/3Aukn1LRr8E-keenan-project?sharecode=n-zKUt88qBWdWxl2yJnVIr2T8bXMJyDw5_o9UnI9P-s

## Project Images

### Full Circuit
![Full Circuit](images/full-circuit.png)

### Motor Control Circuit
![Motor Control](images/motor-control.png)

### Tinkercad Simulation
![Tinkercad Simulation](images/tinkercad-simulation.png)

## Code
The Arduino source code used to control the system is included in this repository.
