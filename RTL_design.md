### 1. What is port?
In electrical circuit theory, a port is a pair of terminals connecting an electrical network or circuit to an external circuit, as a point of entry or exit for electrical energy. A port consists of two nodes (terminals) connected to an outside circuit. The ports are points where input signals are applied or output signals taken.

### 2. What is STD_LOGIC_VECTOR in vhdl?
The std_logic_vector type is used for arrays of std_logic variables and signals. e.g. a 2*4 decoder can have a STD_LOGIC_VECTOR(1 downto 0) instead of separate input ports.

### 3. What is STD_LOGIC_VECTOR vs bit_Vector?

### 4. What does direct bit string mean?
A direct bit string means you write the bits directly in the code, instead of taking them from an input port.

Example of a direct bit string:
```
SLL_OUT <= "10110110" sll 2;
```
Here, "10110110" is the direct bit string

### 5. Explain sll vs sla.

