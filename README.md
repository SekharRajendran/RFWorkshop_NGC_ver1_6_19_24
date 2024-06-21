# RFWorkshop_NGC_ver1_6_19_24
 MathWorks RF Workshop Aero

[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=SekharRajendran/RFWorkshop_NGC_ver1_6_19_24)

# Workshop: Top-Down Design of an RF Receiver and Antenna FrontEnd Integration

This example designs an RF receiver for a ZigBee®-like application using a top-down methodology. It verifies the error rate performance after the addition of impairments such as interfering signals and the integration of the antenna front-end. The example uses the RF Budget Analyzer App to rank the elements contributing to the noise and non-linearity budget, and the Antenna Designer App to design the antenna.

## Specifications

### ZigBee-like System Specifications
- **Data rate**: 250 kbps
- **Modulation**: OQPSK with half sine pulse shaping, as specified in IEEE® 802.15.4 for the physical layer of ZigBee
- **Direct sequence spread spectrum**: Chip rate = 2 Mchips/s
- **Sensitivity specification**: -100 dBm
- **Bit Error Rate (BER) specification**: 1e-4
- **Analog to digital converter (ADC)**: 10 bits and 0 dBm saturation power

### Receiver Specifications
- **Noise Figure (NF)**: 10.7 dB
- **Gain (G)**: 51.5 dB

## Workshop Exercises

### Exercise 1
- **Objective**: Starting from the receiver Gain and Noise Figure, design and analyze a cascade of RF components and integrate them in the system-level model.
- **Tasks**:
  - Design the cascade of RF components.
  - Integrate the components into the system-level model.
  - Measure the corresponding Chip Error Rate (ChER) in the presence of an out-of-band interfering signal.

### Exercise 2
- **Objective**: Integrate a simple dipole antenna into the system-level model of the RF receiver.
- **Tasks**:
  - Integrate the dipole antenna.
  - Understand the impact of polarization mismatch.

### Exercise 3
- **Objective**: Design a dual-polarized antenna, analyze its performance using EM analysis, and integrate it into the system-level model of the RF receiver.
- **Tasks**:
  - Design a dual-polarized antenna.
  - Perform EM analysis on the antenna.
  - Integrate the antenna into the system-level model.
  - Design a Wilkinson combiner and integrate it together with the dual-polarized antenna into the system-level model.

### Exercise 4
- **Objective**: Design a 90-degrees phase shifter and implement it on a PCB together with the Wilkinson combiner.
- **Tasks**:
  - Design a 90-degrees phase shifter.
  - Implement the phase shifter and Wilkinson combiner on a PCB.
  - Analyze the PCB structure using electromagnetic analysis.
  - Verify the system performance in terms of ChER.
