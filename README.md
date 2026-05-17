# Ahmed Khalaf
Hardware / Robotics Engineer

Fresh graduate specializing in:
- PCB Design (Altium)
- Embedded Systems
- Robotics
- Computer Vision

---

# Projects

# Topside Communication Unit (TCU)

<img src="HardwarePortfolio/Topside Control Unit/TCU ASSEMBLY.png" width="650">

4-layer communication and processing PCB designed as the upper board in a stacked two-board robotic system. Acts as the central communication hub, interfacing sensors, cameras, wireless modules, and CAN networks.

### Key Features
- ESP32-WROOM-32 main controller
- Dual CH340G for simultaneous programming/debugging
- Dual CAN nodes using MCP2515 + TJA1050
- HC-12 + nRF24L01 wireless redundancy
- 4 analog camera inputs via RJ45
- 5V → 3.3V regulation with protection circuitry

### Design Highlights
- 4-layer stackup (Sig / GND / Power / Sig)
- Differential routing for CAN and camera signals
- ESD and overcurrent protection
- Mechanically stackable with lower TPU board

<img src="HardwarePortfolio/Topside Control Unit/TCU PCB.png" width="650">

# Topside Power Unit (TPU)

<img src="HardwarePortfolio/Topside Power Unit/TPU PCB.png" width="650">

A dual-input power management and distribution PCB designed as the central power hub of a multi-board robotic system.

The TPU handles high-voltage input regulation, protected power distribution, current monitoring, and relay-based switching for system-level power control.

---

## Key Features

- Dual input rails: 48V + 12V with polyfuse protection and transient suppression
- ACS712 for real-time current monitoring up to ±30A
- Relay-switched 48V output with opto-isolated driver (PC817 + transistor stage)
- AMS1117 for low-voltage rail generation
- Multiple regulated 12V and 5V outputs for subsystems
- USB Type-A power distribution for embedded compute modules
- LED rail indicators for debugging and diagnostics

---

## Design Highlights

- Mixed-voltage power architecture (48V / 12V / 5V / 3.3V)
- Electrical isolation between control and power switching stages
- Protection: polyfuses + varistors + flyback suppression
- Star-style power distribution to subsystems
- Designed in :contentReference[oaicite:2]{index=2}

---

<img src="HardwarePortfolio/Topside Power Unit/TPU SCHEMATIC.png" width="650">

---

# Contact
Email: your@email.com
LinkedIn: your-link
GitHub: your-link
