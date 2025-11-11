# 🌟 RISC-V SoC Tapeout – Week-6: Comprehensive physical design workshop covering the OpenLANE RTL-to-GDSII flow on Sky130 — from floorplanning and cell design to final layout and timing closure.

<div align="center">

![Physical Design](https://img.shields.io/badge/Physical_Design-Workshop-blue?style=for-the-badge)
![OpenLANE](https://img.shields.io/badge/OpenLANE-Flow-green?style=for-the-badge)
![Sky130](https://img.shields.io/badge/Sky130-PDK-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

</div>

🔄 This week marks the **Physical Design Workshop**, where I execute the complete **RTL-to-GDSII implementation** flow using **OpenLANE** and **Sky130 PDK**. Building upon synthesis, timing, and floorplanning concepts from earlier weeks, I now focus on practical physical design. This phase demonstrates how digital and mixed-signal blocks transform from RTL descriptions into verified, fabrication-ready silicon layouts.

---

## 🎯 Objective

> 💡 **Mission:** Master the complete RTL-to-GDSII physical design flow through hands-on implementation

<div align="center">

| 🎓 Learn | 🛠️ Build | ✅ Verify |
|---------|---------|----------|
| Physical design concepts | Standard cells & layouts | DRC, LVS, STA |

</div>

The main goal of this week is to perform a series of **hands-on physical design labs** using a **pre-configured VDI image**. Through these labs, I aim to understand how various stages—standard cell design, layout generation, routing, DRC, and STA—fit together in a complete digital design implementation.

---

### 🎯 Key Milestones

- 🔸 **Setup & Environment:** Configure OpenLANE and Sky130 toolchain
- 🔸 **Synthesis to Layout:** Transform RTL into physical design
- 🔸 **Custom Cell Design:** Create and characterize standard cells
- 🔸 **Timing Closure:** Achieve timing requirements through STA
- 🔸 **Final Verification:** Complete DRC/LVS checks and generate GDSII

---

## 💡 Learning Importance

### 🔍 **Why This Matters**

This workshop connects all the concepts from the previous weeks and provides a real understanding of:

🔹 How **digital design integrates with custom analog and mixed-signal blocks**

🔹 The relationship between **layout design, timing closure, and DRC rules**

🔹 How **physical implementation** influences chip performance and reliability

🔹 The complete flow from **synthesis → STA → layout → verification**


### 🎓 **Skills You'll Gain**

✨ OpenLANE Flow Mastery

✨ Sky130 PDK Understanding

✨ Layout Design Skills

✨ Timing Analysis Expertise

✨ Verification Techniques

✨ Industry-Standard Workflow

> 📌 **By the end of this week**, the complete RTL-to-verified-layout transformation process will be fully understood and documented. I should have a clear view of how an RTL design is transformed into a verified layout ready for fabrication. 

---

## 🧱 Workshop Overview

<div align="center">

### 📅 Five-Day Structured Learning Path

</div>

| **Day** | **Topic** | **Focus Area** | **Key Tools** | **Status** |
|---------|-----------|----------------|---------------|------------|
| **[Day 1](./Day1_Inception_OpenSourceEDA_OpenLANE_Sky130/readme.md)** 🚀 | Inception of Open-Source EDA | Understanding the OpenLANE environment and Sky130 PDK | OpenLANE, Magic | 🟢 |
| **[Day 2](./Day2_GoodFloorplan_vs_BadFloorplan_and_LibraryCells/readme.md)** 📐 | Floorplanning Concepts | Comparing good vs bad floorplans and exploring library cells | OpenLANE, Magic | 🟢 |
| **[Day 3](./Day3_Design_LibraryCell_Magic_ngspice/readme.md)** 🔬 | Standard Cell Design | Creating and characterizing a cell using Magic and Ngspice | Magic, Ngspice | 🟢 |
| **[Day 4](./Day4_LVS_Parasitics/readme.md)** ⏱️ | Timing Analysis & Clock Tree | Running pre-layout STA and learning about clock tree synthesis | OpenSTA, OpenLANE | 🟢 |
| **[Day 5](./Day5_Final_steps_for_RTL2GDS_using_tritonRoute_and_openSTA/readme.md)** 🏁 | Routing & Sign-off | Completing the RTL-to-GDS flow with TritonRoute and OpenSTA | TritonRoute, OpenSTA | 🟢 |

### 📂 Repository Structure

```
Week6_Physical_Design_Workshop/
│
├── 📁 Day1
│   ├── readme.md
│   └── images/
│
├── 📁 Day2
│   ├── readme.md
│   └── images/
│
├── 📁 Day3
│   ├── readme.md
│   └── images/
│
├── 📁 Day4
│   ├── readme.md
│   └── images/
│
└── 📁 Day5
    ├── readme.md
    └── images/
├── .gitignore
├── LICENSE
├── 📄 README.md
│
```

> 💾 Each day has its own folder containing detailed documentation with **screenshots** and **visuals**.

---


