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

## 🛠 Features
- FSM architecture using **Enable-Based Next State FSM (EBNFSM)**.
- Coin recognition in **$0.25 increments**: $0.25 → $0.50 → $0.75.
- Idle and reset handling for robust operation.
- Clean, modular Verilog implementation for maintainability.
- **Testbench included** for simulation verification.

---

## 📂 Repository File Map

| Category | File | Description |
|----------|------|-------------|
| **Main Code** | [VendingMachine_FSM.txt](code/VendingMachine_FSM.txt) | Core FSM logic |
| | [VendingMachine_FSM_Top.txt](code/VendingMachine_FSM_Top.txt) | Top-level design integration |
| | [VendingMachine_ClockDivider.txt](code/VendingMachine_ClockDivider.txt) | Clock divider module |
| | [VendingMachine_Disp_Hex_Mux.txt](code/VendingMachine_Disp_Hex_Mux.txt) | Display driver for 7-seg multiplexing |
| | [VendingMachine_Constraints.txt](code/VendingMachine_Constraints.txt) | FPGA pin constraints |
| **Testbenches** | [FSM Testbench 1](code/VendingMachine_FSM_Testbench_1.txt) | Simulation for normal purchase |
| | [FSM Testbench 2](code/VendingMachine_FSM_Testbench_2.txt) | Simulation for combo purchase |
| **Reports** | [Public Report (Recruiter-Friendly)](report/FSM_Vending_Machine_Report_Public.pdf) | Visual + concise |
| | [Full Academic Report](report/FSM_Vending_Machine_Report_Academic.pdf) | Honors project submission |
| **Diagrams** | [State Diagram](report/FSM_VendingMachine_StateDiagram.pdf) | FSM states & transitions |
| | [Timing Diagrams](report/FSM_VendingMachine_Verification_TimingDiagrams.pdf) | Simulation verification |
| | [Schematic](report/FSM_VendingMachine_Schematic.pdf) | Hardware block-level schematic |

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

## ▶️ How to Run the Project

### 🖥 Simulation
1. Open **Vivado** and create a new project.
2. Add the `.txt` files from `/code` (rename to `.v` when importing).
3. Add the testbench file.
4. Run **Behavioral Simulation**.
5. Check waveform to verify correct FSM behavior.

### ⚡ FPGA Deployment
1. **Download full project**:
   - [📦 vending_machine_fsm_full_project.zip](code/vending_machine_fsm_full_project.zip)
2. **Extract the ZIP**:
   - Windows: Right-click → "Extract All"
   - macOS: Double-click to unzip
3. Open the `.xpr` Vivado project file.
4. Click **Generate Bitstream** ⚙️.
5. Connect the **Nexys A7 board** via USB.
6. Click **Program Device** → Select generated `.bit` file.

### 🛠 Troubleshooting
- ❌ **Bitstream fails to generate?**
  - Ensure correct **Constraints (.xdc)** file is included.
- ❌ **Display not working?**
  - Check 7-seg wiring matches the constraints file.
- ❌ **States stuck?**
  - Reset FPGA and verify pushbutton inputs.

---

## 🎥 Demo
[![Watch the demo](https://img.youtube.com/vi/mEfpK1brveU/0.jpg)](https://youtu.be/mEfpK1brveU)

---

## 👤 Author
**Abid Ahmad**  
Electrical & Computer Engineering, Wayne State University  
🌐 [LinkedIn](https://www.linkedin.com/in/abid-ahmad-83bb0527b)
