# ⚙️ Accelerator and Wrapper Design – SoC-Based Exponential Engine

## 📘 Project Overview
This project focuses on designing and implementing a **hardware accelerator** for computing exponential functions, along with a **wrapper** that enables scalable integration within a **System-on-Chip (SoC)** environment. The goal is to explore parallel computation, interface management, and FPGA-based deployment.

---

## 🔧 Key Components

### 1️⃣ Exponential Engine (Core Accelerator)
- Accepts a **16-bit input**, computes:
  - **Integer part**
  - **Fractional part**
- Outputs exponential result via **fixed-point representation**
- Tested using **ModelSim** and synthesized in **Quartus II**
- Analyzed using **Timing Analyzer** to determine:
  - Maximum operating frequency
  - Combinational delay
  - Resource utilization

---

### 2️⃣ Exponential Accelerator Wrapper
- Wraps the Exponential Engine for **multi-input** operation
- Handles:
  - **Parallel computation** of multiple exponentials
  - **Handshaking protocols** between CPU and accelerator
  - **Data buffering** using FIFO
  - **Control sequencing** via FSM
- Ensures timing overhead is minimized and throughput is maximized

---

### 3️⃣ FPGA Implementation
- Target board: **Cyclone II FPGA**
- Inputs via:
  - Switches (input value)
  - Push-buttons (control signals)
- Outputs via:
  - LEDs (status)
  - Seven-segment display (results)
- Demonstrates:
  - Real-time exponential computation
  - Parallel handling of multiple inputs
  - Validated timing and correctness

---

## 📊 Deliverables

- ✅ Verilog HDL:
  - Exponential Engine module
  - Wrapper logic (FIFO, FSM, controller)
- 🧪 Simulations:
  - ModelSim testbenches with various input cases
- 📈 Synthesis Results:
  - Quartus II timing analysis
  - Area & frequency metrics
- 📄 Report:
  - Integration challenges
  - Parallelism efficiency
  - Frequency scaling insights

---

## 🎓 Course Information

**Course**: Digital Systems Laboratory (Advanced)  
📍 **University of Tehran**  
👨‍🏫 **Supervisor**: Professor Zain Navabi
