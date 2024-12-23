# PWM Generator Circuit using 555 Timer IC

## Overview

This folder contains all the details and resources related to the **PWM Generator Circuit** built using the **555 Timer IC**. The circuit is designed to produce a Pulse Width Modulated (PWM) signal, which is used to control the switching of the MOSFET in all three DC-DC converters:  
1. **Boost Converter**  
2. **Buck Converter**  
3. **Buck-Boost Converter**  

The PWM signal allows precise control of the duty cycle, which directly influences the output voltage in each converter.

---

## Contents of the Folder

1. **Theory File:**  
   - Explains the working principle and design of the PWM generator circuit using the 555 Timer IC.  

2. **Hardware Pictures:**  
   - Includes images of the physical circuit used in the experiment.  

3. **MATLAB Simulation Files:**  
   - Contains the MATLAB file used to simulate the PWM circuit.  

4. **MATLAB Simulation Screenshots:**  
   - Provides visual outputs from the MATLAB simulation of the PWM circuit.

---

## Circuit Details

- The PWM generator circuit is based on the astable mode of the **555 Timer IC**, which generates a continuous train of pulses.  
- By varying the resistance or capacitance in the circuit, the duty cycle of the PWM signal can be adjusted.  
- The generated PWM signal is fed to the gate of the MOSFET in the converters, enabling effective control over their operation.  

---

This folder consolidates all resources related to the PWM generator circuit and demonstrates its integral role in the functioning of the DC-DC converters.
