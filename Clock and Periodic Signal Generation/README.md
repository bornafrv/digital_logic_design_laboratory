# ⏱️ Clock and Periodic Signal Generation – Digital Logic Laboratory

## 📘 Project Overview
This project explores different **clock generation techniques** and **frequency division mechanisms** using a variety of analog and digital components. The focus is on generating stable periodic waveforms and studying their properties such as frequency, duty cycle, and application in sequential logic.

---

## 🔧 Key Components

### 1️⃣ Clock Generators

#### 🌀 Ring Oscillator
- Constructed using **odd-numbered inverters**
- Oscillation frequency depends on **gate propagation delay**
- Used to **estimate inverter delay**

#### 🔋 LM555 Timer (Astable Mode)
- Configured to generate **square waves**
- Frequency and duty cycle determined by RC values:
f = 1.44 / ((R1 + 2×R2) × C)

#### 🔀 Schmitt Trigger Oscillator (74HCT14)
- Provides **clean square wave** output using hysteresis
- Frequency defined by feedback loop and capacitor charging curve

---

### 2️⃣ Frequency Divider using Counters
- Synchronous binary counters divide input clock:
- ÷2, ÷4, ÷8, etc.
- Useful for creating **multi-frequency clocks** from one input

---

### 3️⃣ Flip-Flop-Based Clock Dividers

#### 🔁 T Flip-Flop
- Toggles state on each clock pulse
- Provides **50% duty cycle**

#### 🔁 D Flip-Flop
- Used with feedback logic to implement toggle behavior

---

## 📊 Deliverables

- ✅ Construction of:
- LM555, ring oscillator, Schmitt trigger oscillator
- Flip-flop-based and counter-based dividers
- 📈 Measurement:
- Clock frequency (Hz)
- Duty cycle (%)
- Waveform screenshots via oscilloscope
- 📄 Final report including:
- Circuit schematics
- Measured vs. theoretical values
- Design considerations

---

## 🧪 Tools Used

- Breadboard + ICs (LM555, 74HC14, 74LS76, 74LS90, etc.)
- Oscilloscope for waveform observation
- Function generator and multimeter (for verification)
- Simulation tools (e.g., Proteus, Multisim)

---

## 🎓 Course Information

**Course**: Digital Logic Design Laboratory  
📍 **University of Tehran**  
👨‍🏫 **Instructor**: Prof. Zain Navabi
