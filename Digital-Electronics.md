# 1. What is Gray code?
Gray code is a special binary numbering system where only one bit changes at a time between consecutive numbers.
It is also called Reflected Binary Code (RBC).

# 2. Why is gray code needed?
Gray code is needed in systems where changing multiple bits at the same time can cause errors.
In normal binary counting, multiple bits may change simultaneously.
E.g in Binary:
| Decimal | Binary |
| ------- | ------ |
| 3       | 011    |
| 4       | 100    |

Here, all 3 bits changed at once.
During real electronic switching, tiny timing differences can create errors or false readings.
Gray code reduces this problem because only one bit changes at a time.
Example in Gray code:
| Decimal | Gray Code |
| ------- | --------- |
| 3       | 010       |
| 4       | 110       |

Only one bit changes.
# 3. Describe binary to gray conversion.
### Rule:
MSB (first bit) remains same
Remaining bits = XOR of adjacent binary bits
### Formula:
G<sub>​i</sub> = B<sub>i</sub> ⊕B<sub>i-1</sub>
Where:
B = Binary bits
G = Gray code bits
⊕ = XOR operation

### Example:
Convert Gray 1110 to Binary
Gray: 1 1 1 0

First binary bit = 1

1 XOR 1 = 0
0 XOR 1 = 1
1 XOR 0 = 1

Binary = 1011

# 4. What are the applications of Gray Code?
- ### Rotary Encoders
  Used in Motors, Robotics, Industrial machines. Prevents wrong position readings during transitions.

- ### Karnaugh Maps (K-Maps)
 Adjacent cells in K-maps follow Gray code ordering so only one variable changes between neighboring cells.

- ### Digital Communication
  Helps reduce transmission errors.

- ### Analog to Digital Converters (ADCs)
 Used to minimize switching errors.
