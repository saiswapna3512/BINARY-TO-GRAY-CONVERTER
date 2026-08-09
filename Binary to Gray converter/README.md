# 4-Bit Binary to Gray Code Converter using Verilog

## Description

This project implements a 4-bit Binary-to-Gray Code Converter using Verilog HDL.

Gray Code is a binary numeral system in which two successive values differ by only one bit.

## Conversion Formula

For a 4-bit binary input:

```text
G3 = B3
G2 = B3 XOR B2
G1 = B2 XOR B1
G0 = B1 XOR B0
```

## Example

```text
Binary = 1011
Gray   = 1110
```

## Files

* `binary_to_gray.v` — Verilog design module
* `binary_to_gray_tb.v` — Verilog testbench
* `README.md` — Project documentation
* `.gitignore` — Git ignore file

## Simulation

Compile using Icarus Verilog:

```bash
iverilog -o binary_to_gray_sim binary_to_gray.v binary_to_gray_tb.v
```

Run the simulation:

```bash
vvp binary_to_gray_sim
```

The testbench generates a `binary_to_gray.vcd` waveform file that can be viewed using GTKWave.

## Tools Used

* Verilog HDL
* Visual Studio Code
* Icarus Verilog
* GTKWave

## Features

* 4-bit Binary input
* 4-bit Gray Code output
* Combinational logic
* XOR-based conversion
* Complete testbench
* All 16 input combinations tested

## Author

Add your name here.

