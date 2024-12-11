# 4-BIT-ALU
This project is based on designing a 4 bit Arithmetic Logic Unit using Virtuoso in Cadence Software

This repository contains the design of a **4-bit Arithmetic and Logic Unit (ALU)**. The ALU performs a variety of logical and arithmetic operations based on the input control signals.

## Operations

The ALU is designed to perform the following operations:

### Logical Operations:
- **OR**
- **AND**
- **XOR**

### Arithmetic Operations:
- **Addition**
- **Subtraction**
- **Division**

### Control Signals:
The operations are selected based on a combination of the following control signals:

- **S1, S0 (2-bit control lines)**: These signals control the selection of the operation. The operations corresponding to different values of S1 and S0 are:
  - **00**: OR
  - **01**: AND
  - **10**: XOR
  - **11**: Addition, Subtraction, or Division (depending on C)

- **C (1-bit mode select)**: This control signal determines whether the operation is logical or arithmetic:
  - **C = 0**: Logical operations (OR, AND, XOR)
  - **C = 1**: Arithmetic operations (Addition, Subtraction, Division)

## Selection of Components

To implement the ALU, **multiplexers** were chosen as the core components due to their simplicity, versatility, and ability to select between multiple inputs based on control signals. The following multiplexers were selected:

- **4:1 Multiplexer**: Used to select one of the four operations (OR, AND, XOR, ADD/SUB/DIV) based on the 2-bit control input (**S1, S0**).
- **2:1 Multiplexer**: Used to choose between arithmetic or logical operations based on the **mode select signal (C)**.

## Design Visualizations

Here are the visual representations of the 4-BIT ALU:

### 1. ALU Block Diagram
![ALU Block Diagram](https://github.com/Synisterflare02/4-BIT-ALU/blob/main/img1.png)

### 2. ALU Logic Circuit
![ALU Logic Circuit](https://github.com/Synisterflare02/4-BIT-ALU/blob/main/img2.png)

### 3. ALU Truth Table
![ALU Truth Table](https://github.com/Synisterflare02/4-BIT-ALU/blob/main/img3.png)

## How to Use

Clone the repository to access the design files:

```bash
git clone https://github.com/Synisterflare02/4-BIT-ALU.git
```

Once you have the repository, you can open the design files and explore the ALU functionality. The control signals can be modified to observe how the ALU performs different operations.

## Features:
- Supports both logical and arithmetic operations.
- Uses multiplexers to select operations based on control signals.
- Simple and efficient design suitable for educational purposes.

---

