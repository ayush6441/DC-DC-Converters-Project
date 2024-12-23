# Buck-Boost Converter: Specifications and Observations

## Hardware Specifications

The following components were used in the hardware implementation of the Buck-Boost Converter. Their specifications and characteristics are detailed below:

- **Battery: 9V**  
  A **Super Heavy Duty 1604S 6F22 9V battery** was used as the input voltage source.  

- **Inductor: 20mH**  
  The inductor was custom-made using a **ferrite toroid core** with a relative permittivity of approximately 6.  
  - The core was wound with **38 turns** of thin copper wire, approximately **0.3 mm in diameter**.  
  - The wire type is common **enameled copper wire**.

- **Capacitor: 47µF**  
  A **Radial Electrolytic Capacitor** with a capacitance of **47µF** and a voltage rating of **100V** was used.  

- **Load Resistance: 100Ω**  
  A **100Ω carbon film resistor**, commonly identified by its **color-coded bands**, was used as the load resistance.  

- **MOSFET:**  
  An **N-type MOSFET (IRFZ44N)** was used to control the switching operation of the converter.  

- **Diode:**  
  An **IN4007 general-purpose rectifier diode** was used in the circuit. This diode is capable of withstanding a peak reverse voltage of **1000V** and a maximum forward current of **1A**.

- **PWM Circuit:**  
  The gate pulse for the MOSFET was generated using a **555 timer-based PWM circuit**. The duty cycle values were calculated theoretically as no equipment was available for direct measurement.

---

## Observations and Readings

The input voltage (Vs) was constant at **9V** for all measurements. The output voltage (Vo) and duty cycle (D) were recorded under various conditions and are presented in the table below:

| **S.No.** | **Source Voltage (Vs)** | **Output Voltage (Vo)** | **Duty Cycle (D)** |
|-----------|---------------------------------|----------------------------------|-------------------------|
| 1         | 9V                              | 1.2V                            | 11.76%                 |
| 2         | 9V                              | 2.9V                            | 24.37%                 |
| 3         | 9V                              | 4.6V                            | 33.82%                 |
| 4         | 9V                              | 8.5V                            | 48.57%                 |
| 5         | 9V                              | 15.7V                           | 63.56%                 |
| 6         | 9V                              | 28.3V                           | 75.87%                 |
| 7         | 9V                              | 32.8V                           | 78.47%                 |
| 8         | 9V                              | 52.4V                           | 85.34%                 |
| 9         | 9V                              | 67.3V                           | 88.2%                  |

---

## Key Insights

1. The output voltage (Vo) increased with the duty cycle (D) but did not exceed **67.3V**, indicating a limitation in the converter's performance, possibly due to component ratings or circuit design constraints.  
2. The calculated duty cycles provided accurate control of the output voltage within the design limits of the components.  
3. Heating losses in the MOSFET and inductor can occur during prolonged operation, as no heat sinks were incorporated to manage thermal dissipation.  
4. Proper selection of inductor and capacitor values ensures stable operation and efficient voltage regulation.  

---
