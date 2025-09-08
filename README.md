# Reliable Data Transfer Protocols: P4 & Selective Repeat

This repository contains the implementation and analysis of **reliable data transfer protocols** as part of a networking project. The focus is on **P4 (Programming Protocol-Independent Packet Processors)** and **Selective Repeat ARQ (Automatic Repeat reQuest)**.  

The project explores protocol behavior, error handling, and performance under different simulated network conditions.

---

## 📂 Project Structure
code texts/

│── p4 code.txt # P4 implementation of protocol logic

│── sr code.txt # Selective Repeat protocol implementation



---

## 🚀 Features
- **P4-based implementation** for programmable data-plane packet processing.
- **Selective Repeat ARQ protocol** written in structured code format.
- Analysis of packet retransmission, error handling, and throughput.
- Documentation report (`.pdf`) explaining methodology and results.

---

## ⚙️ Requirements
- **P4 Compiler / Behavioral Model (bmv2)**
- **Python 3.x** (if running simulations)
- Networking tools such as:
  - `mininet`
  - `Wireshark` (for packet inspection)

---

## 🛠️ Usage

### 1. Running the P4 Code

# Example workflow with P4 behavioral model
- p4c --target bmv2 --arch v1model p4_code.p4 -o build/
- simple_switch --log-console build/p4_code.json
2. Running the Selective Repeat Simulation
If the sr code.txt is intended for simulation in C/Python:

# Convert file extension first (if needed)
mv "sr code.txt" sr_protocol.py

# Run simulation
python3 sr_protocol.py

📊 Expected Output
- Packet transmission and retransmission logs.
- Performance evaluation of P4 vs SR ARQ.
- Insights into error control efficiency and protocol behavior.
