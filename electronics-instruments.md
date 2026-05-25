# 1. What is an electronic instrument?
An electronic instrument is a device used to measure, test, generate, analyze, or monitor electrical/electronic signals and parameters.

Examples:
- Oscilloscope
- Multimeter
- LCR meter
- Spectrum analyzer
- SMU
  
---

# 2. Why are electronic instruments important?
Electronic instruments help engineers:
- Design circuits
- Debug systems
- Verify performance
- Ensure safety
- Improve product quality
 
---

# 3. What is accuracy?
Closeness to true value

---

# 4. What is precision?
Repeatability of measurement

---

# 5. What is resolution?
The smallest change an instrument can detect

---

# 6. What is a multimeter used for?
A multimeter measures:
- Voltage
- Current
- Resistance

Some models can also measure:
- Frequency
- Capacitance
- Temperature
- Continuity

---

# 7. What is digit and count in multimeter?
## Digit:
It tells how many numbers the multimeter the can display.
E.g. a A 3½ digit multimeter usually displays from 0000 to 1999.
## Half digit:
The leftmost digit (most significant bit) cannot show full 0–9. Usually it only shows 0 or 1.
## Count:
It's a measure of displayable precision that represents display resolution.
E.g. a 3½ digit multimeter typically has 2000 counts which means display will be from 0 to 1999.

---

# 8. What is the working principle of multimeter?
Converting electrical quantities (V, I, R) into a measurable voltage signal.
When measuring voltage, Red (higher potential) and Black (lower reference) are connected to pass a tiny current against known high resistance (≈ 10 MΩ or more), then, V=IR is calculated across the component (parallel).
Current is measured by inserting a low-value shunt resistor and measuring voltage drop across it by connecting multimerter in series with circuit.
For resistance, multimeter applies a small internal voltage and measures current, then calculates resistance. Power is turned off as otherwise Multimeter’s test voltage and External circuit voltage might clash and give wrong reading.

---

# 9. What is an oscilloscope?
An oscilloscope is an electronic test instrument used to display electrical waveforms versus time.

It helps analyze:
- Signal shape
- Frequency
- Noise
- Rise time
- Distortion
   
---

# 10. Differenciate between analog, digital and mixed oscilloscope.

| Feature | Analog Oscilloscope | Digital Oscilloscope (DSO) | Mixed Signal Oscilloscope (MSO) |
|---|---|---|---|
| Working Principle | Directly displays analog voltage on CRT | Converts signal into digital samples using ADC | Combines digital oscilloscope + logic analyzer |
| Signal Type | Analog signals only | Mainly analog signals | Analog + digital signals |
| Display Technology | CRT | LCD/LED display | LCD/LED display |
| Storage Capability | Usually no waveform storage | Can save waveforms | Can save analog and digital data |
| Signal Processing | Minimal | Advanced digital processing | Advanced mixed-signal analysis |
| Digital Channels | No | Usually no dedicated digital channels | Yes |
| Logic Analysis | Not available | Limited | Available |
| Triggering Features | Basic | Advanced | Advanced protocol triggering |
| Measurements | Manual | Automatic measurements | Automatic measurements + protocol decoding |
| Serial Bus Analysis | No | Limited in some models | Yes |
| Best For | Simple analog waveform viewing | General electronics debugging | Embedded system debugging |
| Common Usage | Old labs, education | Electronics testing and R&D | MCU/FPGA/embedded debugging |
| Complexity | Simple | Moderate | Advanced |
| Cost | Lower (older technology) | Medium | Higher |

---

# 11. What is bandwidth in an oscilloscope?
Bandwidth is the maximum frequency an oscilloscope can accurately measure.

---

# 12. What is a spectrum analyzer?
A spectrum analyzer displays signal amplitude versus frequency.

Used for:
- RF analysis
- EMI testing
- Wireless communication debugging

---

# 13. What is sampling rate?

Sampling rate is the number of samples taken per second when digitizing a signal.
Unit: Samples/second (Sa/s)

---

# 14. What is Vector Network Analyzer?

A VNA measures RF network parameters like S parameters, gain compression, IMD, Harmonic distortion, noise, VSWR etc.
Used for:

- Antenna testing
- RF filters
- Cable testing
- Microwave circuits

---

# 15. What are S-parameters?
S-parameters describe how RF signals behave in a network.

S11	Reflection at input
S21	Forward transmission, port 1 to 2
S12	Reverse leakage
S22	Reflection at output

---

# 16. What is IMD?
Intermodulation distortion occurs when 2 or more signals at different frequencies pass through a non linear device like amplifier or mixer. They are not only amplified / modified but unwanted frequency are created, combining with original signal.

---

# 17. What is a non linear device?
An electronic component whose output is not directly proportional to its input i.e. y≠kx , unlike an Ideal resistor (V=IR) or Small-signal amplifier. E.g. In a diode, conduction barely happens until 0.7 V for silicon. Then current rises rapidly. So, Its current-voltage curve is exponential, not straight.

---
# 18. What is Harmonic distortion?
Higher frequency harmonics can increase heating and skin effect (tendency of AC current to flow mainly near surface). When a pure sine wave is fed to a device, ideally, the output should also be a sine wave at same frequency. But in real life, output often contains extra frequencies that are integer multiples of the original input frequency.
E.g.: When giving pure sine wave input of 1KHz frequency, output should also be 1 kHz. But in a non-linear system, extra frequencies appear, like 2 kHz (2nd harmonic), 3 kHz (3rd harmonic) etc.

---

# 19. Diffentiate between oscilloscope, spectrum analyzer and Vector Network Analyzer.

| Feature | Oscilloscope | Spectrum Analyzer | VNA |
|---|---|---|---|
| Domain | Time domain | Frequency domain | Network (S-parameters) |
| X-axis | Time | Frequency | Frequency |
| Y-axis | Voltage | Power (dBm) | Reflection / transmission |
| Measures | Signal shape | Frequency content | RF behavior of networks |
| Used for | Digital & analog circuits | RF signals | RF components & systems |
| Input type | Electrical signal | RF signal | RF ports (2-port/4-port) |
| Impedance measurement | Absent | Absent | Indirectly Possible |

---

