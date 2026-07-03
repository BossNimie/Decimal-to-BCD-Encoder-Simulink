# Decimal-to-BCD-Encoder-Simulink
A MATLAB Simulink implementation of a Decimal (0–9) to 4-bit Binary Coded Decimal (BCD) encoder using comparators, logic gates, and multiplexers without MATLAB programming.
# README.md

# Decimal to 4-Bit BCD Encoder Using MATLAB Simulink

## Overview

This project presents the design and implementation of a Decimal-to-BCD Encoder in MATLAB Simulink. The model converts decimal digits from 0 to 9 into their corresponding 4-bit Binary Coded Decimal (BCD) representation using standard Simulink blocks only.

The project demonstrates fundamental digital electronics concepts such as combinational logic design, Boolean implementation, data encoding, and simulation-based verification.

---

## Objectives

* Design a decimal-to-BCD encoder using Simulink blocks.
* Convert decimal numbers (0–9) into their equivalent 4-bit BCD outputs.
* Demonstrate the implementation of digital logic without MATLAB programming.
* Explore practical applications of BCD encoding in control systems and embedded systems.

---

## Simulink Blocks Used

* Counter Limited
* Compare To Constant
* Logical Operator (AND)
* Logical Operator (OR)
* Mux
* Display
* Scope (Optional)
* Constant Blocks (Optional)

---

## Methodology

### Step 1: Generate Input

A Counter Limited block generates decimal values from 0 to 9.

Parameters:

* Upper Limit: 9
* Initial Count: 0
* Sample Time: 1 second

### Step 2: Determine Each BCD Bit

A = 1 for decimal values 8 and 9.

B = 1 for decimal values 4, 5, 6, and 7.

C = 1 for decimal values 2, 3, 6, and 7.

D = 1 for decimal values 1, 3, 5, 7, and 9.

### Step 3: Implement Logic

Compare To Constant blocks check the input value, while AND and OR gates implement the Boolean conditions required for each BCD bit.

### Step 4: Display Output

The four output bits are combined using a Mux block and displayed.

---

## Truth Table

| Decimal | A | B | C | D |
| ------- | - | - | - | - |
| 0       | 0 | 0 | 0 | 0 |
| 1       | 0 | 0 | 0 | 1 |
| 2       | 0 | 0 | 1 | 0 |
| 3       | 0 | 0 | 1 | 1 |
| 4       | 0 | 1 | 0 | 0 |
| 5       | 0 | 1 | 0 | 1 |
| 6       | 0 | 1 | 1 | 0 |
| 7       | 0 | 1 | 1 | 1 |
| 8       | 1 | 0 | 0 | 0 |
| 9       | 1 | 0 | 0 | 1 |

---

## Expected Outputs

| Decimal Input | BCD Output |
| ------------- | ---------- |
| 0             | 0000       |
| 1             | 0001       |
| 2             | 0010       |
| 3             | 0011       |
| 4             | 0100       |
| 5             | 0101       |
| 6             | 0110       |
| 7             | 0111       |
| 8             | 1000       |
| 9             | 1001       |

---

## Applications

* Human-Machine Interface (HMI)
* Real-Time Clock (RTC)
* Digital clocks
* Embedded systems
* Seven-segment display interfacing
* Industrial control systems
* Data acquisition systems

---

## Future Improvements

* Design a multi-digit BCD encoder.
* Interface with FPGA hardware.
* Develop a BCD-to-seven-segment decoder.
* Integrate with a digital control system.

---

## Author

Ekujumi Toluwanimi

Electrical and Electronics Engineering 

Interested in:

* Control Systems
* Embedded Systems
* Digital Electronics
* Power Systems
