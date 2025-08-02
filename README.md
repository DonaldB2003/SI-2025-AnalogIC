# SI-2025-Analaog_IC_DESIGN-SU
 🗄️ Repository for summer internship 2025 "Analog and IC Design"
 
 ![IMG-20250618-WA0005](https://github.com/user-attachments/assets/aade2f12-c887-4d1d-a7f1-78660075a613)
 
# 📝 Abstract
This repository documents my summer internship journey (June 2025) at Silicon University’s Advanced VLSI Lab, focusing on the design, simulation, and layout of Analog Integrated Circuits (ICs). The program emphasized hands-on learning with industry-standard tools, covering everything from device physics to post-layout verification. The highlight was the design and analysis of a two-stage CMOS operational amplifier, equipping me with practical skills for a career in VLSI and semiconductor technology.

# 📚 Introduction
Participating in the Analog Integrated Circuit (IC) Design Summer Internship 2025 (SI-2025-AnalogIC) at Silicon University, with hands-on experience in analog IC design using tools such as Xschem, Ngspice, and the Skywater 130nm PDK. The internship includes daily tutorials, assignments, and mentorship from faculty and industry professionals, emphasizing a blend of theoretical learning and practical application to develop core skills relevant to the semiconductor industry.

# 🏛️ Internship Details
- Venue: Room 656, 5th Floor, New Admin Building, Silicon University 🏢
- Duration: June 2nd – June 20th, 2025 📆
- Timings: 10:00am–1:00pm, 2:30pm–5:30pm ⏰
- Resource Persons: Dr. Saroj Rout, Prof. Prasant Swain, Mrinal Das 👨‍🏫

# Course Outcome
 - Skill development in analog IC design workflow from concept to layout
 - Experimental understanding of device behavior and circuit simulation
 - Exposure to open-source industry-relevant EDA toolchains


## 🧠 What is Analog IC Design?

Analog IC Design is a branch of electronics engineering focused on designing integrated circuits that process continuous signals, such as voltage, current, or frequency. Unlike digital circuits that handle binary logic (0s and 1s), analog circuits deal with real-world, varying signals like audio, radio waves, or sensor outputs.

### 🔍 Why Analog IC Design?
- Real-World Interface: Bridges the gap between physical signals and digital systems
- Power Efficiency: Crucial for low-power and high-performance applications
- Signal Fidelity: Maintains the accuracy of sensitive signals, like ECG or RF

### Typical Applications
- 🎧 Audio amplifiers
- 📡 RF front-ends (radios, wireless systems)
- 🔋 Power management (LDOs, DC-DC converters)
- 📷 Sensor readout circuits (e.g., image or temperature sensors)
- 🔗 Signal conversion (ADC/DAC interfaces)

## 🛠️ Tools Used
<ul>
    <li>Magic VLSI, Xschem, ngspice (Open-source EDA) 🧰</li>
    <li>Python/Matlab (Data analysis) 📊</li>
    <li>Skywater 130nm PDK 🏭</li>
</ul>

## 🎤 What is a MEMS Microphone?

A MEMS microphone (Micro-Electro-Mechanical Systems microphone) is a tiny microphone built using semiconductor fabrication techniques. It converts acoustic pressure (sound) into an electrical signal using a microscale diaphragm and capacitive sensing—all integrated on a silicon chip.

<img width="778" height="410" alt="MEMS" src="https://github.com/user-attachments/assets/725762a8-2163-4d5c-a789-c7044905ab21" />


### 💡 How It Works

A thin diaphragm vibrates when sound waves hit it.
These vibrations change the capacitance between the diaphragm and a fixed backplate.
An integrated ASIC (Application-Specific Integrated Circuit) senses this change and outputs an electrical signal, either analog or digital.

### 🏗️MEMS USB Microphone
![MEMS_MIC](https://github.com/user-attachments/assets/7eb3705e-a672-40be-91d9-1d0d5f5f77fa)

- **SPL to Pressure Conversion**:

$Pressure (Pa) = 10^{\frac{60 - 94}{20}} = 19.95 \times 10^{-3} \ Pa$

- **Output Voltage (Peak):**

$V_{out(peak)} = 2 \times 19.95 \times 10^{-3} \times 10^{\frac{-44}{20}} = \mathbf{0.178 \ mV_{pk}}$


#### Schematic

<img width="1799" height="917" alt="image" src="https://github.com/user-attachments/assets/6ba7c98e-0302-4851-8ae8-2d3180e895bf" />


### Laplace-Domain Analysis of Microphone

<img width="1314" height="1401" alt="laplace domain analysis" src="https://github.com/user-attachments/assets/5af73271-55a6-467e-9dee-e5887c5fae1c" />

## Thevenin Equivalent Circuit Model of a MEMS Microphone

<img width="2774" height="1387" alt="Thevenin's Model of a Microphone" src="https://github.com/user-attachments/assets/c99deb69-3d43-4ae8-af3a-bea33cc86961" />
This schematic models a MEMS microphone using its Thevenin equivalent: an AC voltage source in series with a 380 Ω output resistance. The signal is AC-coupled and amplified through an inverting op-amp configuration with a band-pass response. It includes ngspice commands for operating point and future frequency-domain simulation.




## Theveninn equivalent using Op-Amp

<img width="1621" height="1158" alt="Thevenin's equivalent using Op-Amp" src="https://github.com/user-attachments/assets/37db54cb-9307-450b-a132-db497e6ed540" />


## High pass circuit using Op-Amp

### Schematic

<img width="1363" height="855" alt="highpass_filter" src="https://github.com/user-attachments/assets/ab780edc-712d-4e7b-b685-8d48bacb5b22" /> 

### Output

<img width="1400" height="1069" alt="highpass_output" src="https://github.com/user-attachments/assets/74cbdb36-ea5b-45b2-a093-702d57220e88" />

#### High-Pass Filter Cutoff Frequency

Formed by capacitor C₁ = 4.7 µF and resistor R₁ = 5 kΩ.

$$ f_c (\text{Hz}) = \frac{1}{2\pi R_1 C_1} $$

$$ f_c = \frac{1}{2\pi \times 5 \times 10^{3} \times 4.7 \times 10^{-6}} \approx \mathbf{6.77\,Hz} $$

✅ Cutoff Frequency ≈ 6.77 Hz
Blocks DC and very low frequencies, passes voice-range signals.

## Current Mirror Circuit
<img width="1773" height="762" alt="current_mirror" src="https://github.com/user-attachments/assets/94286940-de73-4dc8-9144-bf944e2fec47" />

## Design of Differential amplifier
<img width="1250" height="727" alt="image" src="https://github.com/user-attachments/assets/cc1c3e06-8b4b-426a-8961-ded35e4035c5" />

## NMOS OP-AMP
![nmos_opam](https://github.com/user-attachments/assets/1779587d-028b-48a4-b763-809f5eab6ea1)


# Siliwiz

<img width="1766" height="858" alt="siliwiz2" src="https://github.com/user-attachments/assets/62d275b7-ed63-4add-8714-af72448bd30d" />

SiliWiz is a free, browser-based educational tool that visualizes how semiconductors and integrated circuits are fabricated at the polygon level. It allows users to draw transistor layouts (NMOS, PMOS), resistors, capacitors, and even CMOS logic gates—and instantly view the SPICE simulation and extracted results

# 🔌 Interfacing MEMS Microphone with Digilent Analog Discovery 2

In this experiment, the Digilent Analog Discovery 2 was employed to capture and analyze the analog output of a MEMS microphone. The microphone was connected using jumper wires to the device’s analog input channels. Real-time waveforms produced by ambient sound were visualized using the WaveForms software. This configuration enabled observation of the microphone’s signal behavior and facilitated analysis of its frequency response.


   ## ✅ Tools Used:

  - MEMS Analog Microphone
  - Digilent Analog Discovery 2
  - WaveForms Software
![digilent](https://github.com/user-attachments/assets/3a70df90-69ef-428d-bd38-f8ea4dcb81f5)

- Waveform Software Simulation using Digilent Analog Discovery
  - Generating a sinewave of 1000 Hz
![waveform](https://github.com/user-attachments/assets/3dd2fafe-b54b-4908-9a27-eabe600fe93d)



# 📚 Resources

## Useful Docs:
- [Skywater PDK Manual](https://github.com/silicon-vlsi/SI-2025-AnalogIC/blob/main/docs/skywater-pdk-readthedocs-io-en-main.pdf)
- [OPA344 Datasheet](https://www.ti.com/lit/ds/symlink/opa344.pdf)
- [MEMS Microphone Datasheet](https://cdn.sparkfun.com/assets/0/5/8/b/1/SPH8878LR5H-1_Lovato_DS.pdf)
- [Schematic: Sparkfun breakout board](https://cdn.sparkfun.com/assets/7/5/6/e/d/SparkFun_Analog_MEMS_Microphone_Breakout_SPH8878LR5H-1.pdf)
- [SI-2025-AnalogIC](https://github.com/silicon-vlsi/SI-2025-AnalogIC)
- Schematic/Layout Tutorials (Xschem, ngspice, Magic)



# 🙏 Acknowledgments:
This program would not have been possible without the guidance and support of my mentors *Dr. Saroj Rout* and teammates .Your expertise and encouragement have been instrumental in my learning and development.

Here is the link of full course described by Dr. Saroj Rout https://github.com/silicon-vlsi/SI-2025-AnalogIC


# 📄 License
MIT License

“Analog design is where art meets engineering.” 🎨⚙️

