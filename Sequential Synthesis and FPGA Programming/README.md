# 🔄 Multi-channel Serial Transmitter (MSSD) – Sequential Synthesis & FPGA

## 📘 Project Overview
This project involves the **design, simulation, and FPGA implementation** of a **Multi-channel Serial Transmitter (MSSD)** using **Finite State Machines (FSMs)** and other sequential logic components. The design demonstrates the use of state-driven communication protocols, control logic, and real-time data routing via an FPGA.

---

## 🔧 Key Components

### 1️⃣ Multi-Channel Serial Transmitter (MSSD)
- A synchronous **serial demultiplexer**.
- Detects `1 → 0` edge as **start condition**.
- Serial stream contains:
  - **Port number**
  - **Data size**
  - **Payload bits**
- Output is routed to the correct channel (LEDs), based on port address.

---

### 2️⃣ RTL Design Modules

#### 🧠 Finite State Machine (FSM)
- Implements control logic for decoding the input serial stream and routing output.

#### 🔁 Shift Registers & Demux
- Shift registers:
  - Store destination port, data size, and actual data
- Demultiplexer:
  - Routes data to one of multiple output ports (e.g. LEDs)

#### 🕹 OnePulser
- Generates one-clock-cycle enable pulse used for controlled timing.

#### 🔢 Seven-Segment Display
- Displays the number of bits transmitted to each output port in real-time.

---

### 3️⃣ FPGA Implementation

- **Target Device**: Cyclone II (Altera/Intel)
- **Inputs**:
  - Push-buttons (CLK, RESET)
  - Switches (Serial data input)
- **Outputs**:
  - LEDs (per-channel data output)
  - 7-segment display (bit count)
- **Tools Used**:
  - Quartus II (for synthesis and programming)
  - ModelSim (for behavioral simulation)

---

## 📊 Deliverables

- 🧾 Verilog code for:
  - FSM controller
  - Shift registers
  - One-pulser
  - Demux
  - Display controller
- 🖥 Simulation waveforms (ModelSim)
- 📈 Synthesis report (logic usage, timing, area)
- 🔌 FPGA demonstration: working MSSD logic with real hardware

---

## 🎓 Course Info

**Course**: Digital Systems Laboratory  
📍 **University of Tehran**  
👨‍🏫 **Supervisor**: Professor **Zain Navabi**
