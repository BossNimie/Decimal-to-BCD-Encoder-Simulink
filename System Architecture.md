# System_Architecture.md

# System Architecture

## System Description

The Decimal-to-BCD Encoder is a combinational digital system that converts decimal input values into a 4-bit BCD output.

## Block Diagram

```text
Counter Limited
        │
        ▼
Compare To Constant Blocks
        │
        ▼
AND / OR Logic Gates
        │
        ▼
      Mux Block
        │
        ▼
 Display / Scope
```

## Data Flow

1. The counter generates decimal numbers.
2. Comparator blocks detect specific values.
3. Logic gates generate the individual BCD bits.
4. The Mux combines the four bits.
5. The Display block presents the final output.

## System Requirements

* MATLAB Simulink
* Standard Simulink library blocks
* Personal computer capable of running MATLAB

## Performance

The system produces correct BCD outputs for all decimal values from 0 to 9 with negligible computational delay due to the simplicity of the logic network.
