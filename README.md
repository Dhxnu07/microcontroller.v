# 8-Bit Microcontroller in Verilog

This is a simple 8-bit microcontroller written in Verilog. It has an ALU, data memory, program memory, control logic, and a register set.

## 🧠 Features
- 8-bit Accumulator
- 12-bit Instructions
- ALU (Add, Subtract, AND, OR)
- Separate Program & Data Memory
- 4-stage FSM: LOAD → FETCH → DECODE → EXECUTE

## 📂 Files
- `MicroController.v`: Top-level module
- `ALU.v`: Arithmetic unit
- `DMem.v`: Data memory
- `PMem.v`: Program memory
- `Control_Logic.v`: FSM controller

## 🧪 How to Simulate
1. Load instructions into `program_mem.dat`
2. Use a Verilog simulator like Icarus:
   ```bash
   iverilog -o mcu MicroController.v ALU.v ...
   vvp mcu
