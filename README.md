## Variable Frequency Drive (VFD) Using Arduino UNO
This project implements a simple Variable Frequency Drive (VFD) using an Arduino UNO. It generates a sine-modulated PWM signal using a lookup table and allows motor speed (RPM) control via serial input. The Arduino computes the necessary output frequency based on the desired RPM and applies the corresponding switching frequency for SPWM (Sinusoidal Pulse Width Modulation).

## Features
1. Adjustable motor RPM through Serial Monitor.
2. Frequency calculation mapped from RPM (assuming a 4-pole motor by default).
3. Dynamic switching frequency toggling between 5kHz and 15kHz.
4. Uses Timer1 in fast PWM mode to generate high-resolution SPWM signals.
5. Lookup table for efficient sine wave generation.
6. Compatible with IRFZ44N MOSFETs, IGBT, and TLP250 gate drivers.

## Hardware Requirements
1. Arduino UNO
2. 4 x IRFZ44NPBF (MOSFETs)
3. 4 x TLP250H(F) (Gate Driver ICs)
4. B1212S-1W isolated DC-DC converters for gate drive power
5. Passive components (resistors, capacitors)
6. Power supply: 12V DC input
7. Output filter: Inductor + Capacitor
8. Motor (AC Induction Motor).
