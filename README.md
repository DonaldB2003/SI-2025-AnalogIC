# 🛠️ SI-2025-AnalogIC-Design Internship
## 📝 Abstract
This repository documents my summer internship journey (June 2025) at Silicon University’s Advanced VLSI Lab, focusing on the design, simulation, and layout of Analog Integrated Circuits (ICs). The program emphasized hands-on learning with industry-standard tools, covering everything from device physics to post-layout verification. The highlight was the design and analysis of a two-stage CMOS operational amplifier, equipping me with practical skills for a career in VLSI and semiconductor technology.

## 📚 Introduction
Analog ICs are the backbone of real-world signal processing, powering applications from sensor interfaces to communications. This internship offered a structured exploration of analog design, blending theory with practical labs using Cadence Virtuoso, LTspice, and open-source EDA tools.

## 🏛️ Internship Details
Venue: Room 656, 5th Floor, New Admin Building, Silicon University 🏢
Duration: June 2nd – June 20th, 2025 📆
Timings: 10:00am–1:00pm, 2:30pm–5:30pm ⏰
Resource Persons: Dr. Saroj Rout, Prof. Prasant Swain, Mrinal Das 👨‍🏫

## 🗂️ Table of Contents
<ul>
    <li>Project Overview</li>
    <li>Design Flow</li>
    <li>Tools Used</li>
    <li>ab Modules</li>
    <li>Results & Analysis</li>
    <li>How to Run</li>
    <li>Resources</li>
    <li>Acknowledgements</li>
    <li>License</li>
</ul>

## 🚀 Project Overview
The internship covered the complete analog IC design flow:

📐 Specification & Topology Selection

📝 Schematic Entry

⚡ Simulation (DC, AC, transient, noise)

🧩 Layout & Verification (DRC, LVS)

🔬 Post-Layout Simulation

## 🔄 Design Flow
text
graph TD;
    A[Specification] --> B[Schematic Design]
    B --> C[Simulation]
    C --> D[Layout]
    D --> E[DRC/LVS]
    E --> F[Post-Layout Simulation]
    F --> G[Documentation]


## 🛠️ Tools Used
<ul>
    <li>Cadence Virtuoso (Schematic/Layout) 🖥️</li>
    <li>-LTspice (Simulation) ⚡</li>
    <li>Magic VLSI, Xschem, ngspice (Open-source EDA) 🧰</li>
    <li>Python/Matlab (Data analysis) 📊</li>
    <li>Skywater 130nm PDK 🏭</li>
</ul>

## 🧪 Lab Modules
### Lab 1: CMOS Inverter Design
Schematic and DC transfer characteristics

![CMOS Inverter Schematic](https://github.com/silicon-vlsi/SI-2025-AnalogIC/raw/main/images/inverter 2: Current Mirror

Simple and cascode current mirrors

![Current Mirror Layout](https://github.com/silicon-vlsi/SI-2025-AnalogIC/raw/main/images/current 3: Differential Pair

Biasing, common-mode, and differential-mode gain

### Lab 4: Two-Stage Op-Amp
Schematic, frequency response, phase margin

![Op-Amp Schematic](https://github.com/silicon-vlsi/SI-2025-AnalogIC/raw/main/images/opamp_s 5: Layout of Analog Cells

Matching techniques, parasitic extraction

![Analog Cell Layout](https://github.com/silicon-vlsi/SI-2025-AnalogIC/raw/main/images/analog 6: Comparator Design

Offset, speed analysis, transient simulation

### Lab 7: Automation Scripts
Python scripts for batch simulation and plotting

## 📈 Results & Analysis
|Metric	Target	|Pre-Layout	|Post-Layout|
|-----------------|-----------|-----------|
|DC Gain (dB)|	>60|	72|	68|
|UGB (MHz)	|>10	|15	|13.5|
|Phase Margin (°)|	>60|	75	|70|
|Power (µW)|	<500|	420|	430|
Offset (mV)	|<5	|2.1	|2.5|

Sample simulation plot:

![Gain vs Frequency Plot](https://github.com/silicon-vlsi/SI-2025-AnalogIC/raw/main/images/gain_plot.png to Run

Clone this repository.

Open schematic/layout files in Cadence Virtuoso or LTspice.

Follow /docs/layout_instructions.md for DRC/LVS.

Run simulation scripts in the /scripts folder.

## 📚 Resources
### Textbooks:
<ul>
    <li>T. C. Carusone, D. A. Johns, K. A. Martin, Analog Integrated Circuit Design</li>
    <li>John P. Uyemura, CMOS Logic Circuit Design</li>
    <li>R. Jacob Baker, CMOS: Circuit Design, Layout, and Simulation</li>

### Useful Docs:
<ul>
    <li>Skywater PDK Manual</li>
    <li>OPA344 Datasheet</li>
    <li>Schematic/Layout Tutorials (Xschem, ngspice, Magic)</li>
</ul>


## 🙏 Acknowledgments:
This program would not have been possible without the guidance and support of my mentors *Dr. Saroj Rout* and teammates .Your expertise and encouragement have been instrumental in my learning and development.

Here is the link of full course described by Dr. Saroj Rout https://github.com/silicon-vlsi/SI-2025-AnalogIC


## 📄 License
MIT License

“Analog design is where art meets engineering.” 🎨⚙️

