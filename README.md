![Electronics](https://img.shields.io/badge/Electronics-darkred)

![Hardware](https://img.shields.io/badge/Hardware-blue)

# Two Switch Flyback Converter
Design and implementation of a 50W dual-switch flyback power converter. Calculated components' values, performed efficiency and stability analysis in MATLAB, and simulated the process in PLECS.

This was a project done for the "Power Electronics" course at EPFL

Authors: Arkadiusz Rozmarynowicz, Timothée Roth.

## Table of contents.
* [Converter parameters](#converter-parameters)
* [General information](#general-information)
* [Results](#results)
* [Technologies used](#technologies-used)

## Converter parameters.
- Nominal power: 50W
- Output voltage: 5V
- Input voltage: between 30V and 60V, with 50V nominal
- Switching frequency: 320kHz
- Max output voltage ripple: 2%

## General information.
- Calculated device's parameters, such as:
    - duty cycle,
    - coupled inductor's winding ratio, dimensions
    - capacitor and resistor values,
    - MOSFETs and diodes parameters,
    - heatsink size.
- Simulated the circuit in PLECS. Analyzed:
    - compensation network's functioning,
    - impact of input voltage characteristics on output voltage.
- Simulated the system's stability and efficiency in MATLAB.
- Manually wound the coupled inductor.
- Measured the coupled inductor's characteristics, namely:
    - magnetizing and leakage inductance,
    - saturation current,
    - winding resistance.
- Tested the device for efficiency under a range of valid input voltages.

<p align="center">
<img src="./Images/Circuit_From_STMicroelectronics.avif" alt="./Images/Circuit_From_STMicroelectronics.avif" width="650"><br>
<em>Figure 1: Idea schematic. Source: STMicroelectronics.</em>
</p>

<p align="center">
<img src="./Images/View_3D.png" alt="./Images/View_3D.png" width="550"><br>
<em>Figure 2: 3D view of the PCB.</em>
</p>

## Results.
The converter has reached an around 80% efficiency for a range of input voltages from 30V to 60V.

## Technologies used.
- Software:
    - Altium Designer
    - PLECS
    - MATLAB
- Measurement tools:
    - BODE100 analyser
    - Power choke meter
    - IR heat camera