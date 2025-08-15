# 🎯 Vending Machine FSM – Verilog HDL (Honors College Project)

A **Finite State Machine (FSM)** vending machine designed in **Verilog HDL**, supporting incremental coin inputs, multiple product prices, combo purchase logic, and **real hardware testing** on the **Nexys A7 FPGA board**.  
Developed as part of my **Honors College Independent Project** at **Wayne State University**.

---

## 📌 Project Highlights
- Built a **fully custom FSM** from scratch for the honors upgrade.
- Expanded from a 2-product design to **3 products**:
  - 🍬 Candy – $0.25  
  - 🥤 Soda – $0.50  
  - 🍟 Chips – $0.75
- Implemented **combo logic** allowing bundled purchases at $0.75.
- Integrated **LED indicators** for coin progress and dispensing states.
- Verified through **simulation** & **FPGA hardware deployment**.

---

## 🛠️ Features
- FSM architecture using **Enable-Based Next State FSM (EBNFSM)**.
- Coin recognition in **$0.25 increments**: $0.25 → $0.50 → $0.75.
- Idle/reset handling for robust operation.
- Modular Verilog implementation for easy updates.
- **Two testbenches** for simulation verification.

---

## 📂 Repository Structure

| 📁 Folder / File | 📄 Description | 🔗 Direct Link |
|------------------|---------------|----------------|
| **`code/`** | All Verilog source files & testbenches | [View Folder](code/) |
| `VendingMachine_FSM.txt` | Main FSM logic | [Open](code/VendingMachine_FSM.txt) |
| `VendingMachine_FSM_Top.txt` | Top-level module integration | [Open](code/VendingMachine_FSM_Top.txt) |
| `VendingMachine_FSM_Testbench_1.txt` | Testbench – Scenario 1 | [Open](code/VendingMachine_FSM_Testbench_1.txt) |
| `VendingMachine_FSM_Testbench_2.txt` | Testbench – Scenario 2 | [Open](code/VendingMachine_FSM_Testbench_2.txt) |
| `VendingMachine_ClockDivider.txt` | Clock divider module | [Open](code/VendingMachine_ClockDivider.txt) |
| `VendingMachine_Disp_Hex_Mux.txt` | Display multiplexer | [Open](code/VendingMachine_Disp_Hex_Mux.txt) |
| `VendingMachine_Constraints.txt` | XDC constraints file | [Open](code/VendingMachine_Constraints.txt) |
| **`report/`** | Documentation, diagrams & timing analysis | [View Folder](report/) |
| `FSM_VendingMachine_Report_Academic.pdf` | Full academic report | [Open](report/FSM_VendingMachine_Report_Academic.pdf) |
| `FSM_VendingMachine_Verification_TimingDiagrams.pdf` | Timing verification diagrams | [Open](report/FSM_VendingMachine_Verification_TimingDiagrams.pdf) |
| `FSM_VendingMachine_StateDiagram.pdf` | State diagram | [Open](report/FSM_VendingMachine_StateDiagram.pdf) |
| `vending_machine_fsm_full_project.zip` | Full Vivado project | [Download](code/vending_machine_fsm_full_project.zip) |

---

## 🧠 Skills Gained
- **Digital Logic Design** – FSM architecture & state transitions.
- **HDL Proficiency** – Verilog HDL design & debugging.
- **Simulation & Testing** – Vivado simulation flow.
- **FPGA Programming** – Bitstream generation & deployment.
- **System Integration** – From HDL code to physical hardware.

---

## 💻 Tools & Hardware
- **Language**: Verilog HDL
- **IDE**: Vivado Design Suite
- **Hardware**: Digilent Nexys A7 FPGA (Artix-7 100T)

---

## ▶️ How to Run on FPGA
1. **Download & Extract**  
   - Click [here to download ZIP](code/vending_machine_fsm_full_project.zip).  
   - Extract the ZIP using your OS file explorer or `unzip` command:
     ```bash
     unzip vending_machine_fsm_full_project.zip
     ```
2. **Open in Vivado**  
   - Launch **Vivado** → `File` → `Open Project` → Select the extracted `.xpr` file.
3. **Generate Bitstream**  
   - Click **Generate Bitstream** (should succeed without errors if extracted correctly).
4. **Program the FPGA**  
   - Connect Nexys A7 → Open Hardware Manager → `Program Device`.
5. **Test on Hardware**  
   - Insert coins using switches/buttons.  
   - Observe LED indicators & 7-segment display outputs.

---

## 🛠 Troubleshooting
- **Bitstream Fails?** → Ensure all `.xdc` constraints are loaded.
- **Display Issues?** → Verify `VendingMachine_Disp_Hex_Mux.txt` is included in project sources.
- **No Output?** → Check FPGA jumper settings & re-program.

---

## 📄 Documentation
- [📘 Full Academic Report](report/FSM_VendingMachine_Report_Academic.pdf)  
- [⏱ Timing Diagrams](report/FSM_VendingMachine_Verification_TimingDiagrams.pdf)  
- [📍 State Diagram](report/FSM_VendingMachine_StateDiagram.pdf)  

---

## 👤 Author
**Abid Ahmad**  
Electrical & Computer Engineering – Wayne State University  
🌐 [LinkedIn](https://www.linkedin.com/in/abid-ahmad-83bb0527b)

---
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

**[FSM_VendingMachine_Verification_TimingDiagrams.pdf](report/FSM_VendingMachine_Verification_TimingDiagrams.pdf)**

---

## 📍 State Diagram

[![View State Diagram](https://img.shields.io/badge/View%20PDF-State%20Diagram-blue?style=for-the-badge&logo=adobeacrobatreader)](report/FSM_VendingMachine_StateDiagram.pdf)

Click the badge above to view the full PDF of the FSM state diagram.

-----

## 👤 Author
**Abid Ahmad**  
Electrical & Computer Engineering, Wayne State University
🌐 [LinkedIn](https://www.linkedin.com/in/abid-ahmad-83bb0527b) 

---
