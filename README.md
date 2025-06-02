# vending-machine-fsm

This project implements a Finite State Machine (FSM) for a vending machine using Verilog HDL. It accepts coins in $0.25 increments and dispenses a product once the total reaches $0.75. The design includes combo purchase logic, reset functionality, LED-based output display, and a testbench for simulation.

This version of the project was developed as part of my Honors College independent project. It builds upon an earlier design originally created with Valentina Shabi. For the Honors requirement, I extended the design by adding support for an additional coin input and a second product selection logic. All enhancements and simulations were completed independently.

---

## 💡 Features
- Designed using EBNFSM (Enable-Based Next State FSM)
- Accepts coins: 0.25 → 0.50 → 0.75 → 1.00
- Combo switch enables bundled product option
- Two item selection logic
- Handles reset and idle states
- Output feedback displayed using onboard LEDs (coin progress, dispense signal, etc.)
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
1. Open the project in your Verilog simulator (Vivado)
2. Compile `fsm.v` and `testbench.v`
3. Run the simulation and observe the output waveform or testbench logs
