# 1. What is spice?
A node is a point or a continuous conducting path in an electrical circuit where two or more circuit elements are connected. It is a region of a circuit where the voltage is the same.

# 2. What is Node?

# 3. What is E, F, G, H?
E = Voltage-Controlled Voltage Source (VCVS), F = Current-Controlled Current Source (CCCS), G= Voltage-Controlled Current Source (VCCS), H= Current-Controlled Voltage Source (CCVS)

# 4. What is .dat file?
a data file that stores simulation results like waveforms etc

# 5. What is .PROBE?
Saves simulation data for waveform viewing

# 6. What is .OP?
Operating Point Analysis is a DC analysis in PSpice that calculates the steady-state voltages at every circuit node and the currents flowing through the circuit components.

# 7. What is .step?
.step directive allows you to run a simulation repeatedly while varying a component value, a global parameter, a temperature, or a model parameter across a specified range or list. .STEP = parameter variation across repeated simulations.

# 8. What DC sweep?
Time independent simulation. DC Sweep is a type of circuit simulation in which we gradually change the DC voltage or current of a source and observe how the circuit responds.

E.g. We set:
- Start voltage = 0 V
- End voltage = 10 V
- Step size = 1 V

The simulator performs the following:
Input voltage	Current through resistor
0 V	0 mA
1 V	1 mA
2 V	2 mA
3 V	3 mA
4 V	4 mA
5 V	5 mA
...	...
10 V	10 mA

Using Ohm's law:
\[
I=\frac{V}{R}
\]

The simulator calculates the circuit's DC operating condition at every voltage step.The graph shows how the output current changes as the input voltage changes.

# 9. What is node analysis and mesh analysis?
**Nodal analysis** is a method of circuit analysis in which we calculate the voltages at different nodes in a circuit with respect to a reference node (ground). Uses Kirchhoff's Current Law (KCL).

**Mesh analysis** is a method of circuit analysis in which we calculate currents circulating through different meshes (independent loops) of a circuit. It Uses Kirchhoff's Voltage Law (KVL).
