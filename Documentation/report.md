# Summary
The ripple-carry adder computes the sum of two 2-bit binary numbers by combining the outputs of a half adder and full adder, then outputs the sum and carry bit (carryout).

Both a half adder and full adder were constructed before the RCA to demonstrate how they combine to form the RCA.

Diagrams and truth tables for all adders are documented below. At the bottom of this report, you will find example images of the RCA breadboard circuit.

The RCA consists of an 8-pin switch array, an XOR gate, an AND gate, an OR gate, and a 10-LED array. More details on these components are available in the [Materials List](/materials_list.md).

---

# Half Adder

## Truth Table for Half Adder
| A | B | Carry | Sum |
| :---: | :---: | :---: | :---:|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 0 |

## Circuit Diagram for Half Adder
<img src="../Media/ECE%20232%20-%20Half%20Adder-1.jpg" alt="Half Adder Circuit Diagram" width="600">

## Wiring Diagram for Half Adder
<img src="../Media/Half%20Adder%20Diagram.jpg" alt="Half Adder Wiring Diagram" width="800">

---

# Full Adder

## Truth Table for Full Adder
| A | B | C_in | C_out | Sum |
| :---: | :---: | :---: | :---: | :---: |
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 | 1 |
| 0 | 1 | 0 | 0 | 1 |
| 0 | 1 | 1 | 1 | 0 |
| 1 | 0 | 0 | 0 | 1 |
| 1 | 0 | 1 | 1 | 0 |
| 1 | 1 | 0 | 1 | 0 |
| 1 | 1 | 1 | 1 | 1 |

## Circuit Diagram for Full Adder
<img src="../Media/FA.jpg" alt="Full Adder Circuit Diagram" width="600">

## Wiring Diagram for Full Adder
<img src="../Media/Full%20Adder%20Diagram.jpg" alt="Full Adder Wiring Diagram" width="800">

---

# Ripple-Carry Adder (RCA)

## Truth Table for RCA
| A_1 | A_0 | B_1 | B_0 | C_out | S_1 | S_0 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 1 | 0 | 0 | 1 |
| 0 | 0 | 1 | 0 | 0 | 1 | 0 |
| 0 | 0 | 1 | 1 | 0 | 1 | 1 |
| 0 | 1 | 0 | 0 | 0 | 0 | 1 |
| 0 | 1 | 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 0 | 1 | 1 |
| 0 | 1 | 1 | 1 | 1 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 | 1 | 0 |
| 1 | 0 | 0 | 1 | 0 | 1 | 1 |
| 1 | 0 | 1 | 0 | 1 | 0 | 0 |
| 1 | 0 | 1 | 1 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 | 1 | 0 | 0 |
| 1 | 1 | 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 | 1 | 0 |

## Circuit Diagram for RCA
<img src="../Media/ECE%20232%20-%20Lab%204%20-%20Ripple%20Carry%20Adder(1)-1.jpg" alt="RCA Circuit Diagram" width="600">

## Wiring Diagram for RCA
<img src="../Media/2-Bit%20RCA%20Diagram.jpg" alt="RCA Wiring Diagram" width="800">

## Top Down View of RCA
<img src="../Media/2-Input-RCA%20Example.jpg" alt="Example1" width="61000">

## Angled View of RCA
<img src="../Media/extra%20image%20of%20RCA%20for%20documentation.jpg" alt="Example2" width="61000">
