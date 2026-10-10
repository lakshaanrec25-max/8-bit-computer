# 8-Bit Computer Using Verilog HDL

## 1. Project Overview

This project implements a simple 8-bit computer using Verilog HDL. It demonstrates how a CPU fetches, decodes, and executes instructions using registers, memory, an Arithmetic Logic Unit (ALU), and a Control Unit.

The project is developed using Xilinx Vivado and can be tested through behavioral simulation.

## 2. Objectives

- Design a basic 8-bit computer architecture.
- Understand the instruction execution cycle.
- Perform arithmetic and logical operations.
- Learn the functions of registers, memory, and buses.
- Simulate and verify the design using Vivado.

## 3. System Components

### Program Counter (PC)
Stores the address of the next instruction to be fetched.

### Memory Address Register (MAR)
Stores the address of the memory location that the CPU wants to access.

### Instruction Register (IR)
Stores the current instruction for decoding and execution.

### A Register
Stores data used by the ALU during operations.

### B Register
Stores another input value for ALU operations.

### Arithmetic Logic Unit (ALU)
Performs arithmetic and logical operations according to the control signals.

### Control Unit
Generates control signals to coordinate registers, memory, and the ALU.

### RAM
Stores data used during program execution.

### ROM
Stores the program instructions executed by the CPU.

### Output Register
Stores the result that needs to be displayed.

### Seven-Segment Display
Converts output data into signals for displaying values on a seven-segment display.

## 4. Working Principle

The computer operates through the following stages:

1. **Fetch:** The instruction is fetched from program memory.
2. **Decode:** The Control Unit identifies the instruction and required operation.
3. **Execute:** The ALU or another component performs the operation.
4. **Store:** The result is stored in a register or memory.
5. **Display:** The output can be shown through the output display logic.

## 5. Instruction Cycle and T-Cycles

An instruction cycle is the complete process of executing one instruction.

The process is divided into smaller timing steps called T-cycles. Each T-cycle performs a particular part of the operation, controlled by clock timing and control signals.

For example:
- T1: Prepare or fetch the instruction.
- T2: Decode the instruction or prepare required data.
- T3: Execute the required operation.
- T4: Store the result, if required.

The exact number and function of T-cycles depend on the implementation of the Control Unit.

## 6. Internal Bus

A bus is a group of wires used to transfer information between computer components.

- **Data bus:** Transfers data.
- **Address bus:** Carries memory addresses.
- **Control signals:** Coordinate operations such as reading, writing, loading, and enabling registers.

The bus helps the CPU, registers, ALU, and memory communicate with one another.

## 7. Supported Operations

The project includes program modes intended for:

- Addition
- Subtraction
- AND operation
- XOR operation
- Multiplication
- Division
- Fibonacci sequence
- Custom program

Actual functionality should be verified using the simulation results.

## 8. Tools Used

- Verilog HDL
- Xilinx Vivado
- Behavioral Simulation
- FPGA development board, if used for hardware testing

## 9. How to Run the Project

1. Clone or download this GitHub repository.
2. Open Xilinx Vivado.
3. Create or open the project.
4. Add the Verilog source files.
5. Set the appropriate top module.
6. Add the testbench files.
7. Run behavioral simulation.
8. Check the waveform and output values.
9. If using an FPGA board, configure the required pins and program the board.

## 10. Applications

- Learning basic computer architecture.
- Understanding CPU instruction execution.
- Studying Verilog and digital design.
- Demonstrating registers, buses, memory, and ALU operations.
- Practicing FPGA design and simulation.

## 11. Future Improvements

- Add more instructions.
- Improve the instruction execution sequence.
- Add more display options.
- Test the design on an FPGA board.
- Improve error handling and verification.

## 12. Conclusion

This project demonstrates the basic structure and working of an 8-bit computer using Verilog HDL. It provides practical experience with CPU components, instruction execution, data transfer, arithmetic and logical operations, and digital system simulation.

## Team

Developed as part of a hackathon project.
