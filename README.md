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

| **Day** | **Topic** | **Focus Area** | **Key Tools** | **Status** |
|---------|-----------|----------------|---------------|------------|
| **Day_1**  | 🚀 Inception of Open-Source EDA | Understanding the OpenLANE environment and Sky130 PDK | OpenLANE, Magic | 🟢 |
| **Day_2**  | 📐 Floorplanning Concepts | Comparing good vs bad floorplans and exploring library cells | OpenLANE, Magic | 🟢 |
| **Day_3**  | 🔬 Standard Cell Design | Creating and characterizing a cell using Magic and Ngspice | Magic, Ngspice | 🟢 |
| **Day_4**  | ⏱️ Timing Analysis & Clock Tree | Running pre-layout STA and learning about clock tree synthesis | OpenSTA, OpenLANE | 🟢 |
| **Day_5**  | 🏁 Routing & Sign-off | Completing the RTL-to-GDS flow with TritonRoute and OpenSTA | TritonRoute, OpenSTA | 🟢 |

</div>

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

## 🧰 Lab Setup

<div align="center">

### 🖥️ Virtual Development Infrastructure (VDI)

![VirtualBox](https://img.shields.io/badge/VirtualBox-7.2.4-183A61?style=flat&logo=virtualbox)
![Ubuntu](https://img.shields.io/badge/Ubuntu-18.04_LTS-E95420?style=flat&logo=ubuntu)
![Storage](https://img.shields.io/badge/Storage-~100GB-red?style=flat)
![RAM](https://img.shields.io/badge/RAM-4GB+-orange?style=flat)

</div>

The labs for this week are done using a **pre-configured VDI image** provided as part of the workshop.

### 🔗 Download Links

#### 📦 **Physical Design Tools VDI Image**

```
Platform: VirtualBox
Format: .vdi
OS: Ubuntu 18.04 LTS (64-bit)
Pre-installed: All required tools
```

🔽 **[Download VDI File](https://drive.google.com/file/d/1Ri30Yeqjyprv-rStHEScUMpKtw2JfVJe/view)**

#### 🛠️ **OpenLANE Tools Package**

```
Size: ~100 GB
Format: .zip
Contents: Complete OpenLANE toolchain
Includes: Sky130 PDK
```

🔽 **[Download openlane.zip](https://vsd-labs.sgp1.cdn.digitaloceanspaces.com/vsd-labs/openlane.zip)**

> ⚠️ **Important:** Ensure you have at least **100 GB of free disk space** before downloading

---

### 🪟 Setup on Windows

#### Step-by-Step Guide

**Step 1️⃣: Install Oracle VirtualBox**

```
🔗 Download from: https://www.virtualbox.org/wiki/Downloads
📦 Choose: Windows hosts
💿 Install: Follow the installation wizard
```

**Step 2️⃣: Create New Virtual Machine**

1. 🖱️ Open VirtualBox
2. ➕ Click **"New"** to create a new VM
3. ⚙️ Configure the following:
   ```
   Name: Physical_Design_Workshop
   Type: Linux
   Version: Ubuntu (64-bit)
   ```

**Step 3️⃣: Memory Allocation**

```
Recommended: 4096 MB (4 GB)
Minimum: 2048 MB (2 GB)
Optimal: 8192 MB (8 GB) if available
```

**Step 4️⃣: Select Virtual Hard Disk**

- 🔘 Choose **"Use an existing virtual hard disk file"**
- 📂 Click the folder icon to browse
- 📁 Navigate to your extracted `.vdi` file
- ✅ Select it and confirm
- ➡️ Then click **Start**

---

### 🐧 Setup on Ubuntu

#### Installation Commands

**Step 1️⃣: Install VirtualBox**

```bash
# Update package repository
sudo apt update

# Install VirtualBox
sudo apt install virtualbox

# Verify installation
virtualbox --help
```

**Step 2️⃣: Launch VirtualBox**

```bash
# Start VirtualBox GUI
virtualbox &
```

**Step 3️⃣: Create Virtual Machine**

```
1. Click "New" button
2. Name: Physical_Design_Workshop
3. Type: Linux
4. Version: Ubuntu (64-bit)
5. Click "Next"
```

**Step 4️⃣: Configure Memory**

```
Memory Size: 4096 MB (recommended)
Click "Next"
```

**Step 5️⃣: Add Existing Virtual Disk**

```bash
# Select "Use an existing virtual hard disk file"
# Browse to extracted .vdi file
# Click "Create" and Start the VM
```

---

### 🔧 Pre-installed Tools Overview

<div align="center">

| Tool | Purpose | Version | Documentation |
|------|---------|---------|---------------|
| 🔨 **OpenLANE** | RTL-to-GDSII Flow | Latest | [Docs](https://openlane.readthedocs.io/) |
| 🎨 **Magic** | Layout Editor & DRC | 8.3+ | [Guide](http://opencircuitdesign.com/magic/) |
| ⚡ **Ngspice** | SPICE Simulator | 34+ | [Manual](http://ngspice.sourceforge.net/) |
| ⏱️ **OpenSTA** | Static Timing Analysis | Latest | [Docs](https://github.com/The-OpenROAD-Project/OpenSTA) |
| 🛣️ **TritonRoute** | Detailed Router | Latest | [Info](https://github.com/The-OpenROAD-Project/TritonRoute) |
| 📚 **Sky130 PDK** | Process Design Kit | v1.0+ | [PDK Docs](https://skywater-pdk.readthedocs.io/) |

</div>

> ✅ **All tools are pre-configured** in the VDI for immediate lab access

---

### 📸 Screenshot Guidelines

> 🎯 **Quality Requirements:**
> - ✅ Clear and readable terminal text
> - ✅ Complete window capture (with username/timestamp)
> - ✅ Annotated when necessary
> - ✅ Organized in `images/` subfolder

---

## 🧠 Learning Outcomes

### 🎓 By the end of **Week 6**, I aim to:

#### 🛠️ **Technical Skills**

✅ Successfully set up and use the Physical Design VDI environment

✅ Perform end-to-end **RTL-to-GDSII implementation** using OpenLANE and Sky130

✅ Design and characterize a standard cell using **Magic** and **Ngspice**

#### 🔍 **Analysis Capabilities**

✅ Understand **clock tree synthesis** and its impact on timing

✅ Master **pre-layout STA** techniques and methodologies

✅ Comprehend **routing concepts** and optimization strategies

#### 🌟 **Holistic Understanding**

✅ Connect all stages of digital design — from **RTL** to **verified layout**

✅ Recognize design trade-offs between **area, power, and performance**

✅ Apply **industry best practices** in physical design

---

## 🙌 Acknowledgements  

👨‍🏫 **Kunal Ghosh** – VSD SoC Program Mentor  

🧑‍🤝‍🧑 **Open-source EDA Community** – Tool contributors & maintainers  

🌍 **RISC-V & Efabless Ecosystem** – Enabling open tapeout programs  

---

## 🎓 Reference and Resources

### 📚 Essential Documentation & Repositories

📘 **Primary Reference** - [SoC Design and Planning (NASSCOM × VSD)](https://github.com/fayizferosh/soc-design-and-planning-nasscom-vsd/)

📙 **OpenLANE Docs** - [Complete flow documentation](https://openlane.readthedocs.io/)

📗 **Sky130 PDK** - [Skywater PDK: Process design kit details](https://skywater-pdk.readthedocs.io/)

📕 **Magic Tutorial** - [OpenCircuitDesign: Layout design guide](http://opencircuitdesign.com/magic/)

📓 **OpenSTA Manual** - [Timing analysis reference](https://github.com/The-OpenROAD-Project/OpenSTA)

---

## 🔗 Repository Links

👉 **Week-0 Repository Link:** https://github.com/CHITTESH-S/Week-0_RISC-V_SoC_TapeOut

👉 **Week-1 Repository Link:** https://github.com/CHITTESH-S/Week-1_RISC-V_SoC_TapeOut

👉 **Week-2 Repository Link:** https://github.com/CHITTESH-S/Week-2_RISC-V_SoC_TapeOut

👉 **Week-3 Repository Link:** https://github.com/CHITTESH-S/Week-3_RISC-V_SoC_TapeOut

👉 **Week-4 Repository Link:** https://github.com/CHITTESH-S/Week-4_RISC-V_SoC_TapeOut

👉 **Week-5 Repository Link:** https://github.com/CHITTESH-S/Week-5_RISC-V_SoC_TapeOut

👉 **Week-7 Repository Link:** https://github.com/CHITTESH-S/Week-7_RISC-V_SoC_TapeOut

👉 **Main Repository Link:** https://github.com/CHITTESH-S/RISC-V_SoC_TapeOut_VSD

👨‍💻 **Contributor**: [Chittesh S](https://github.com/CHITTESH-S)  

---
