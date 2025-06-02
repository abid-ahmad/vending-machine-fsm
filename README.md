# vending-machine-fsm

This project implements a Finite State Machine (FSM) for a simple vending machine using Verilog HDL. It accepts coins in $0.25 increments and dispenses a product once the total reaches $0.75. The design includes combo purchase logic, reset functionality, and a testbench for simulation.

---

## 💡 Features
- Designed using EBNFSM (Enable-Based Next State FSM)
- Accepts coins: 0.25 → 0.50 → 0.75
- Combo switch enables bundled product option
- Handles reset and idle states
- Modular and clean Verilog implementation

---

## 📂 Files Included
- `fsm.v` – Main Verilog FSM module
- `testbench.v` – Verilog testbench to simulate functionality
- *(Optional)* `diagram.png` – State diagram

---

## 🛠️ Tools Used
- Verilog HDL
- Simulated with: Vivado

---

## 👨‍💻 Author
**Abid Ahmad**  
Electrical and Computer Engineering student – Wayne State University

---

## 📎 How to Simulate
1. Open the project in your Verilog simulator Vivado
2. Compile `fsm.v` and `testbench.v`
3. Run the simulation and observe the output waveform or testbench logs
