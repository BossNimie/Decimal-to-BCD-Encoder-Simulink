# Design_Procedure.md

# Design Procedure

## Step 1: Input Generation

A Counter Limited block is used to generate decimal values from 0 to 9 sequentially.

Parameters:

* Upper Limit: 9
* Initial Count: 0
* Sample Time: 1 second

## Step 2: Logic Development

The BCD output bits are generated according to the following conditions:

### Bit A

A = 1 for:

* Decimal 8
* Decimal 9

### Bit B

B = 1 for:

* Decimal 4
* Decimal 5
* Decimal 6
* Decimal 7

### Bit C

C = 1 for:

* Decimal 2
* Decimal 3
* Decimal 6
* Decimal 7

### Bit D

D = 1 for:

* Decimal 1
* Decimal 3
* Decimal 5
* Decimal 7
* Decimal 9

## Step 3: Logic Implementation

Compare To Constant blocks detect the required decimal values. Their outputs are combined using AND and OR gates to generate each BCD bit.

## Step 4: Output Generation

The four BCD bits are combined using a Mux block and displayed using a Display block.

## Step 5: Verification

The output is verified by comparing the generated BCD values with the standard BCD truth table.
