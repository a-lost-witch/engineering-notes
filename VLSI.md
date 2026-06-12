# 1. What is VLSI?
VLSI (Very Large Scale Integration) is a technology used to design and fabricate integrated circuits (ICs) by combining millions or billions of transistors on a single chip.
###Example:
- Microprocessors (Intel, AMD)
- Mobile phone chips (Qualcomm Snapdragon)
- Memory chips (RAM, Flash)

# 2. Describe the Basic Steps in VLSI Design Flow.

# 3. What is Moore’s Law?
The number of transistors on a semiconductor chip doubles approximately every 18 to 24 months, while the cost per transistor decreases.

### Example:
Earlier microprocessors had thousands of transistors
Modern chips have billions of transistors (CPU, GPU, SoC)

# 4. What is CMOS Technology?
CMOS (Complementary Metal-Oxide-Semiconductor) is a technology used to build integrated circuits using both NMOS and PMOS transistors together.

A CMOS circuit uses:
NMOS → strong pull-down (connects to GND)
PMOS → strong pull-up (connects to VDD)

# 5. Why is CMOS widely used?
✔ Very low static power consumption<br>
✔ High noise immunity<br>
✔ High density (more transistors per chip)

# 6. Comparison of MOSFET Regions

| Region | Condition | Behavior |
|----------|----------|----------|
| Cutoff | \(V_{GS}<V_T\) | OFF switch |
| Triode (Linear) | \(V_{GS}>V_T\), \(V_{DS}<V_{GS}-V_T\) | Resistor-like |
| Saturation | \(V_{GS}>V_T\), \(V_{DS}\ge V_{GS}-V_T\) | Current source-like |

# 7. What is triode region in mosfet and why is it called triode?
The **triode region** (also called the **linear region** or **ohmic region**) is the operating region where a MOSFET behaves approximately like a **voltage-controlled resistor**.

For an NMOS, the conditions are:

$$
V_{GS} > V_T
$$

and

$$
V_{DS} < V_{GS} - V_T
$$

where:

- V<sub>{GS}</sub> = Gate-to-Source voltage
- \(V_{DS}\) = Drain-to-Source voltage
- \(V_T\) = Threshold voltage

# 8. Why is PMOS called Pull up and NMOS pull down?
For an NMOS, the source is usually the lowest-voltage terminal.

Suppose:

Source = 0 V (ground)
Gate = 5 V

Then:
V<sub>GS</sub> =5−0=5V

When the NMOS turns ON, a conductive channel forms.
Now the output node and ground are connected.
Since the output node is at a higher electric potential than ground, electrons flow through the NMOS toward ground (equivalently, charge leaves the node).
As charge leaves the output node:
Voltage decreases from 5 V → 4 V → 3 V → 2 V → 1 V → 0 V
which is a perfect logic 0.

Thus "pulling" the voltage down.

Now suppose if an NMOS is connected to pull a node UP toward VDD.

Source = 0 V (since, connected to ground).

As the output rises from 0V to 5V, the voltage difference across the transistor keeps shrinking.
Eventually the output gets stuck at roughly at V<sub>DD</sub>−V<sub>TH</sub> (since, V<sub>DD</sub> has to be positive to pull the electrons) and can never be V<sub>DD</sub>.

This is why NMOS is said to pass a strong 0 but a weak 1 and PMOS has the opposite behavior.
	​

# 9. Explain Latch vs Flip flop.
Latch monitors input as long as enable pin is enabled (level triggered) whereas Flip flop monitors input only when clock pulse changes (edge triggered)

# 10. Explain setup time and hold time in flip flop
Setup time (tsu) is the minimum time that the data input must be stable before the active clock edge for the flip-flop to reliably capture it. Hold time (th) is the minimum time the data input must remain stable after the active clock edge. Violating either constraint causes a metastability condition, where the output may settle unpredictably.


# 11. Explain Metastability.
Metastability is a condition where a flip-flop cannot immediately decide whether to store a 0 or a 1.
It occurs when setup or hold time requirements are violated, causing the output to take an unpredictable amount of time to settle to a valid logic 0 or logic 1.
