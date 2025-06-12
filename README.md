# 🎯 vending-machine-fsm

This project implements a Finite State Machine (FSM) for a vending machine using **Verilog HDL**. It accepts coins in $0.25 increments and dispenses products based on total credit inserted. The design includes combo purchase logic, reset functionality, LED-based output display, and a testbench for simulation.

This version of the project was developed independently for my **Honors College project**. The original version was a team effort (with **Valentina Shabi** and myself), supporting two products: candy ($0.25) and soda ($0.50), with a max of $0.75. For the honors upgrade, I **designed a full FSM from scratch**, added a **third product (chips – $0.75)**, and implemented **complete combo logic**, **state transitions**, and **hardware-based LED feedback**.

✅ The design was **fully tested and deployed on the Nexys A7 FPGA board** with the **Artix-7 100T (XC7A100T-1CSG324C)** chip to verify real hardware behavior and output accuracy.

---

## 💡 Features

- FSM architecture using **Enable-Based Next State FSM (EBNFSM)**
- Accepts coins incrementally: **$0.25 → $0.50 → $0.75**
- Products:
  - 🍬 Candy – $0.25
  - 🥤 Soda – $0.50
  - 🍟 Chips – $0.75
- Combo switch enables bundled product dispensing at $0.75
- Reset and idle state handling
- LED-based outputs showing:
  - Coin progress
  - Dispensing state
- Clean and modular Verilog implementation
- Verified on physical FPGA hardware (Nexys A7)

---

## 📂 Files Included

- `fsm.v` – Main Verilog FSM module
- `testbench.v` – Simulation testbench

---

## 🛠️ Tools Used

- **Language**: Verilog HDL  
- **Simulation**: Vivado Design Suite  
- **Hardware**: Digilent **Nexys A7** FPGA board  
  - Chip: **Xilinx Artix-7 100T (XC7A100T-1CSG324C)**

---

## 👨‍💻 Author

**Abid Ahmad**  
Electrical and Computer Engineering student  
**Wayne State University**

---

## 📎 How to Simulate

1. Open the project in **Vivado**.
2. Add `fsm.v` and `testbench.v` to a new project.
3. Run behavioral simulation.
4. Observe testbench outputs and waveform behavior for verification.

---

## 🎥 Demo Video

[![Watch the demo](https://img.youtube.com/vi/mEfpK1brveU/0.jpg)](https://youtu.be/mEfpK1brveU)

---

## 🧠 What I Learned

- Designing and debugging FSMs in Verilog from scratch
- Translating state diagrams into real-world circuit behavior
- Implementing LED output based on control logic
- Managing edge cases with resets and combos
- Deploying Verilog designs on **real FPGA hardware**
- Importance of modularity and simulation before synthesis
