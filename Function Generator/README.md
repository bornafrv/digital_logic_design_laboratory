# 🎚️ FPGA-Based Function Generator – Digital Systems Lab

## 📘 Project Overview
This project implements a **Function Generator** capable of producing **sine, square, triangle, and custom waveforms** using digital components on an **FPGA board**. The generator uses **Direct Digital Synthesis (DDS)** techniques and outputs signals through **PWM-based Digital-to-Analog Conversion (DAC)**.

Designed and tested as part of the **Digital Systems Laboratory** at the **University of Tehran**, the system enables real-time waveform control through onboard switches and push-buttons.

---

## 🔧 Key Modules

### 1️⃣ Waveform Generator
- Implements **DDS** using a **ROM-based lookup table**
- Outputs supported:
  - Sine wave
  - Square wave
  - Triangle wave
  - Reciprocal waveform
  - Rectified waveforms
- Output is a digital signal ready for PWM conversion

---

### 2️⃣ Digital-to-Analog Conversion (DAC)
- Uses **PWM (Pulse Width Modulation)** for digital-to-analog conversion
- Combined with **RC low-pass filter** to smooth output waveform
- Output suitable for oscilloscope monitoring

---

### 3️⃣ Frequency Selector
- Implements a **counter-based clock divider**
- User-configurable via FPGA switches
- Allows dynamic frequency selection for generated waveforms

---

### 4️⃣ Amplitude Selector
- Modulates waveform amplitude based on switch input
- Multiplies output sample values before DAC stage

---

## 📊 Deliverables

- ✅ Verilog modules for:
  - DDS engine
  - PWM DAC
  - Frequency controller
  - Amplitude modulator
- 📈 Simulations:
  - Testbenches validating waveform logic
- 🖥 Oscilloscope Screenshots:
  - Real output waveforms at various frequencies/amplitudes
- 📄 Final Report:
  - Theoretical background
  - Design breakdown
  - Simulation + FPGA implementation results

---

## ⚙️ Tools Used

- **Quartus II** for synthesis
- **ModelSim** for simulation
- **Oscilloscope** for output verification
- **Cyclone II FPGA Development Board**

---

## 🎓 Course Info

**Course**: Digital Systems Laboratory  
📍 **University of Tehran**  
👨‍🏫 **Instructor**: Prof. Zain Navabi
