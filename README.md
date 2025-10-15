# Edge AI Applications Repository

This repository is the central landing page for **Microchip’s Edge AI application projects**.  
It showcases how AI and ML can be deployed efficiently on **resource-constrained MCUs, MPUs, and FPGAs**, covering a wide range of real-world use cases across **vision, audio, predictive maintenance, HMI, and electrical domains**.  

The goal of this repo is to:
- Provide **reference applications** that engineers can reuse and adapt.  
- Demonstrate **best practices** for deploying models on Microchip hardware.  
- Highlight **cross-platform capabilities** (dsPIC, PIC32, SAM MPU, PolarFire SoC).  
- Serve as a **knowledge base** for teams, customers, and partners building Edge AI solutions.

---

## 🔹 Application Categories

### 1. Vision Applications
Vision is one of the fastest-growing areas in embedded AI. These applications use cameras or image sensors to enable devices to see and interpret their environment.  
Typical challenges include **low-power image capture**, **real-time inference**, and **memory-efficient neural networks**.

Example use cases:
- **Object detection** – identifying objects in a scene (e.g., detecting tools in a factory).  
- **Person presence / people counting** – enabling smart surveillance or occupancy detection.  
- **Anomaly detection** – spotting irregular patterns in video streams for safety monitoring.  

📂 Directory: `applications/vision/`

---

### 2. Audio Applications
Audio-based AI enables devices to listen, understand, and react to sound inputs. These solutions are highly relevant for **hands-free control, monitoring, and assistive technologies**.  
The main challenges are achieving **always-on low-power listening** and **robustness across noisy environments**.

Example use cases:
- **Keyword spotting (KWS)** – detecting short commands like “Hey Microchip” or “Start”.  
- **Voice Activity Detection (VAD)** – distinguishing speech from background noise.  
- **Sound classification** – recognizing events such as glass breaking, alarms, or machinery noise.  
- **Beamforming / multi-mic arrays** – improving signal quality and directionality.  

📂 Directory: `applications/audio/`

---

### 3. Predictive Maintenance Applications
Predictive Maintenance (PdM) brings intelligence to industrial and IoT systems by monitoring equipment health in real-time. Instead of waiting for machines to fail, AI detects early signs of degradation, reducing downtime and cost.  
These applications often use **vibration, current, and acoustic signals** as inputs.

Example use cases:
- **Bearing wear detection** – identifying early signs of mechanical stress.  
- **Motor health monitoring** – detecting imbalance, misalignment, or efficiency loss.  
- **Compressor condition monitoring** – catching leaks or pressure drops before failure.  

📂 Directory: `applications/predictive_maintenance/`

---

### 4. Human–Machine Interface (HMI) Applications
HMI solutions enhance how users interact with devices by making interfaces more **natural, intuitive, and responsive**. AI-powered HMIs go beyond simple buttons, enabling **gesture, touchless, and multimodal interactions**.

Example use cases:
- **Gesture recognition** – enabling touchless controls in consumer electronics or automotive.  
- **Voice UI integration** – combining wake-words with command-and-control systems.  
- **Multimodal HMI** – fusing gesture + voice + context for richer interactions.  

📂 Directory: `applications/hmi/`

---

### 5. Electrical Applications
Electrical signal monitoring is critical in industrial and residential environments. AI enhances traditional electrical sensing by detecting subtle patterns and anomalies that rule-based systems may miss.  
This category includes **safety, efficiency, and grid-monitoring applications**.

Example use cases:
- **Arc fault detection** – identifying hazardous sparks in power lines or appliances.  
- **Load monitoring** – tracking device-level consumption for energy efficiency.  
- **Smart metering & anomaly detection** – predicting faults or abnormal electrical behavior.  

📂 Directory: `applications/electrical/`

---

## 🖥 Supported Platforms

Applications in this repository are optimized for a range of Microchip devices:  

- **dsPIC33A** – Compact DSP-enabled MCUs for real-time signal processing.  
- **PIC32CX** – High-performance MCUs with rich peripherals for connected devices.  
- **SAMA7** – MPU with Arm® Cortex®-A7 and NEON for Linux-based AI.  
- **SAM9X75** – MPU family optimized for low-power embedded Linux.  
- **PolarFire SoC** – FPGA + RISC-V SoC for high-performance, low-power AI acceleration.  

Platform-specific configurations, BSPs, and build instructions will be stored in:  
📂 `platforms/`

---

## 🛠 Toolchains & Build Support

This repository supports multiple build flows, including:  

- **MPLAB X** with XC compilers for MCUs.  
- **Harmony Configurator (MHC)** for driver and middleware setup.  
- **Bare-metal / CMake templates** for lightweight embedded projects.  
- **Libero + VectorBlox SDK** for FPGA-based AI acceleration.  

📂 `toolchains/`

---

## 📊 ML Assets & Pipelines

Reusable ML assets, training/export utilities, and evaluation scripts will be centralized under:  
📂 `ml/`

Contents include:
- **Model cards** – standardized documentation for each model.  
- **Quantized binaries** – INT8, FP16, or custom formats optimized for deployment.  
- **Evaluation scripts** – measuring accuracy, latency, memory footprint, and power.  
- **Pipelines** – training/export flows using TensorFlow Lite Micro, TVM, ONNX2C, etc.  

---

## 🔗 VectorBlox Reference

For FPGA-based acceleration, we will reference the official **[Microchip-VectorBlox GitHub repository](https://github.com/Microchip-Vectorblox)**.  

This ensures continuity and avoids duplication.  
Optionally, VectorBlox may be included as a **submodule** in:  
📂 `vendors/vectorblox/`

---

## 📚 Documentation

General documentation and guides will be found under:  
📂 `docs/`

Planned docs:
- **Overview** of the repo  
- **Getting Started** guides per platform  
- **Roadmap** of upcoming apps  
- **FAQs & troubleshooting**

---

For bug reports, feature requests, or questions, please use the GitHub Issues section.

---

## 📜 License



