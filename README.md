# 🎯 Vending Machine FSM – Verilog HDL (Honors College Project)

A **Finite State Machine (FSM)** vending machine designed in **Verilog HDL**, supporting incremental coin inputs, multiple product prices, combo purchase logic, and **real hardware testing** on the **Nexys A7 FPGA board**.  
Developed as part of my **Honors College independent project** at **Wayne State University**.

---

## 📌 Project Highlights
- Built a **fully custom FSM** from scratch for the honors upgrade.
- Expanded from a 2-product design to **3 products**:
  - 🍬 Candy – $0.25  
  - 🥤 Soda – $0.50  
  - 🍟 Chips – $0.75
- Implemented **combo logic** allowing bundled purchases at $0.75.
- Integrated **LED indicators** for coin progress and dispensing states.
- Verified functionality through **simulation** and **FPGA hardware deployment**.

---

## 🛠️ Features
- FSM architecture using **Enable-Based Next State FSM (EBNFSM)**.
- Coin recognition in **$0.25 increments**: $0.25 → $0.50 → $0.75.
- Idle and reset handling for robust operation.
- Clean, modular Verilog implementation for maintainability.
- **Testbench included** for simulation verification.

---

## 📂 Files in Repository
- `fsm.v` – Main FSM module.
- `testbench.v` – Verilog testbench for simulation.
- State diagram & design notes (if available).

---

## 🧠 Skills Gained
- **Digital Logic Design** – FSM architecture & state transitions.
- **Hardware Description Languages** – Verilog HDL.
- **Simulation & Debugging** – Using Vivado Design Suite.
- **FPGA Deployment** – Programming Nexys A7 (Artix-7 100T) board.
- **Hardware-Software Integration** – Translating logical design to physical outputs.

---

## 💻 Tools & Hardware
- **Language**: Verilog HDL
- **IDE/Simulator**: Vivado Design Suite
- **Hardware**: Digilent Nexys A7 FPGA Board  
  - Chip: **Xilinx Artix-7 100T (XC7A100T-1CSG324C)**

---

## ▶️ How to Simulate
1. Open **Vivado** and create a new project.
2. Add `fsm.v` and `testbench.v` to the project.
3. Run **Behavioral Simulation**.
4. Check the waveform output for correct FSM operation.

---

## 🎥 Demo
[![Watch the demo](https://img.youtube.com/vi/mEfpK1brveU/0.jpg)](https://youtu.be/mEfpK1brveU)

---
## 📄 Documentation

- [**Public Technical Report (Recruiter-Friendly)**](report/FSM_Vending_Machine_Report_Public.pdf) – Clean, visual summary of design, implementation, and FPGA testing results.  
- [**Full Academic Report**](report/FSM_Vending_Machine_Report_Academic.pdf) – Original honors project submission for ECE2610.
---
## ⏱ Timing Diagrams & Verification

## ⏱ Timing Diagrams & Verification
[📄 Click here to view the full PDF](FSM_VendingMachine_Verification_TimingDiagrams.pdf)

---

## 👤 Author
**Abid Ahmad**  
Electrical & Computer Engineering, Wayne State University

---
