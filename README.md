# 16-Bit CPU with Arithmetic, Logic, Relational Operations, Datapath, and Seven-Segment Display

## Project Overview

This project demonstrates the design and implementation of a **16-bit CPU** built using digital logic principles.  
It performs **arithmetic operations, logical operations, and relational comparisons**, and outputs results in real time on **seven-segment displays**.  

The CPU integrates an **Arithmetic Logic Unit (ALU)**, relational comparator circuits, multiplexers, and a complete **datapath** to manage the flow of data between registers, the ALU, and the display.  
This project serves as a foundation for a future **32-bit CPU implementation using VHDL and the MIPS instruction set architecture**.

---

## Folder Structure & Key Components

### Arithmetic Operation Circuit
![Arithmetic Operation Circuit](https://github.com/Ansong-ux/16BitCpu/blob/486c975d3022a7dc139c653cd2d26d83e06557c1/Screenshot_2026-03-26_03_44_25.png)

### Relational Operation Circuit
![Relational Operation Circuit](https://github.com/Ansong-ux/16BitCpu/blob/486c975d3022a7dc139c653cd2d26d83e06557c1/Screenshot_2026-03-26_03_44_49.png)

### Decimal Decoder
![Decimal Decoder](https://github.com/Ansong-ux/16BitCpu/blob/486c975d3022a7dc139c653cd2d26d83e06557c1/Screenshot_2026-03-26_03_45_22.png)

### Control Unit
![Control Unit](https://github.com/Ansong-ux/16BitCpu/blob/486c975d3022a7dc139c653cd2d26d83e06557c1/Screenshot_2026-03-26_03_46_15.png)

### Datapath
![Datapath](https://github.com/Ansong-ux/16BitCpu/blob/486c975d3022a7dc139c653cd2d26d83e06557c1/Screenshot_2026-03-26_03_45_05.png)

### Full CPU
![CPU](https://github.com/Ansong-ux/16BitCpu/blob/486c975d3022a7dc139c653cd2d26d83e06557c1/Screenshot_2026-03-26_03_45_41.png)

---

## Features

### Arithmetic Operations
- Addition
- Subtraction
- Multiplication
- Division

### Logical Operations
- AND
- OR
- XOR
- NOT

### Relational Operations
- Equal (`A == B`)
- Not Equal (`A != B`)
- Greater Than (`A > B`)
- Less Than (`A < B`)
- Greater Than or Equal (`A >= B`)
- Less Than or Equal (`A <= B`)

---

## CPU Architecture

The CPU is built using **modular digital blocks** for clarity, scalability, and ease of future expansion.

### Main Components
- **16-bit Input Registers**  
- **Arithmetic Logic Unit (ALU)**  
- **Relational Comparator Unit**  
- **Multiplexers (MUXes) for selecting data paths**  
- **Control Unit**  
- **Hexadecimal Decoder**  
- **Seven-Segment Display Interface**  

The **datapath** ensures proper flow of data between inputs, computation units, and outputs under the direction of control signals.

---

## Operation Control

The CPU uses **control bits** to select which operation to perform:

| Control Bits | Operation             |
| ------------ | -------------------- |
| 0000         | Addition             |
| 0001         | Subtraction          |
| 0010         | Multiplication       |
| 0011         | Division             |
| 0100         | AND                  |
| 0101         | OR                   |
| 0110         | XOR                  |
| 0111         | NOT                  |
| 1000         | Equal                |
| 1001         | Not Equal            |
| 1010         | Greater Than         |
| 1011         | Less Than            |
| 1100         | Greater Than or Equal|
| 1101         | Less Than or Equal   |

---

## Output Display

The 16-bit output is divided into **four 4-bit nibbles**:

- Bits `[15:12]`  
- Bits `[11:8]`  
- Bits `[7:4]`  
- Bits `[3:0]`  

Each nibble is decoded into hexadecimal and displayed on **seven-segment displays**.

**Example:**  

Binary Result:  
`0000 0000 0001 1010`  

Displayed Output:  
`001A`

---

## Design Methodology

The CPU was built progressively using modular digital design techniques:

1. Design a **single-bit ALU**  
2. Cascade into a **16-bit ALU**  
3. Integrate **arithmetic circuits**  
4. Integrate **logic circuits**  
5. Add **relational comparator circuits**  
6. Connect components through a **datapath**  
7. Use **multiplexers** for operation selection  
8. Split output into **4-bit nibbles**  
9. Decode nibbles to **hexadecimal**  
10. Drive **seven-segment displays**

---

## Tools Used

- **Logisim / Logisim Evolution**  
- **Digital Logic Design Principles**

---

## Future Development

The project is designed to be extended into a more advanced architecture:

- Upgrade from **16-bit to 32-bit CPU**  
- Implement using **VHDL**  
- Integrate **MIPS instruction set architecture**  
- Add **register file and program counter**  
- Include **instruction decoder and memory interface**  
- Complete **datapath and control unit for full CPU**  
- Deploy on **FPGA**

---

## Long-Term Vision

The long-term goal is to develop a complete **32-bit CPU architecture**, combining arithmetic, logic, relational operations, and MIPS instruction support, suitable for FPGA implementation and advanced computer architecture study.

---

## Author

Built by **[Sasu Thomas Ansong ]**
