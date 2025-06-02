# vending-machine-fsm

This project implements a Finite State Machine (FSM) for a vending machine using Verilog HDL. It accepts coins in $0.25 increments and dispenses products based on total credit inserted. The design includes combo purchase logic, reset functionality, LED-based output display, and a testbench for simulation.

This version of the project was developed as part of my Honors College independent project. The original version was created as a team effort (including Valentina Shabi and myself) to support two products: candy ($0.25) and soda ($0.50), with a maximum total of $0.75. For the Honors requirement, I independently designed and implemented a full FSM from scratch, adding a third item—chips ($0.75)—along with complete state transitions, combo logic, LED outputs, and simulation.

The design was fully tested and deployed on an FPGA board to verify real hardware behavior and output accuracy.

---

## 💡 Features
- Designed using EBNFSM (Enable-Based Next State FSM)
- Accepts coins: 0.25 → 0.50 → 0.75
- Products:
  - 🍬 Candy – $0.25
  - 🥤 Soda – $0.50
  - 🍟 Chips – $0.75
- Combo switch enables bundled product option
- Reset and idle state handling
- Output displayed using onboard LEDs (coin progress and product dispensing)
- Fully tested on an FPGA board
- Clean, modular Verilog implementation

---

## 📂 Files Included
- `fsm.v` – Main Verilog FSM module
- `testbench.v` – Verilog testbench to simulate functionality
- *(Optional)* `diagram.png` – State diagram of the FSM

---

## 🛠️ Tools Used
- Verilog HDL
- Simulated with: Vivado
- Hardware tested on: [Specify your FPGA board, if known — e.g., Basys 3]

---

## 👨‍💻 Author
**Abid Ahmad**  
Electrical and Computer Engineering student – Wayne State University

---

## 📎 How to Simulate
1. Open the project in your Verilog simulator (Vivado)
2. Compile `fsm.v` and `testbench.v`
3. Run the simulation and observe the output waveform or testbench logs
