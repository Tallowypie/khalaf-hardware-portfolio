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

# Video & Signal Distribution Breakout Board

<img src="HardwarePortfolio/Camera Board/Camera Board PCB.jpeg" width="650">

A passive signal routing and breakout PCB designed to sit between the TCU and system peripherals, providing structured access to video, camera, and communication signals.

The board acts as a flexible interconnect layer, improving system organization, debugging capability, and reconfigurability during development and testing.

---

## Key Features

- Multi-purpose signal routing between system subsystems (TCU ↔ cameras ↔ communication lines)
- Three main connector groups for IP video, analog video, and communication signals
- Independent analog camera channels (4x) via JST connectors
- solder jumper-based routing for flexible signal path selection
- Support for external/internal video balun configuration per channel
- Structured net naming for scalable system integration

---

## Design Highlights

- Passive routing architecture (no active components)
- Fully reconfigurable signal paths using solder jumpers
- Modular connector system for fast debugging and system rewire
- Designed for testability and rapid bring-up
- Clean signal separation for analog vs digital lines
- Layout optimized for system integration rather than electronics density

---

<img src="HardwarePortfolio/Camera Board/Camera Board Schematic.jpeg" width="650">

---

# Video Balun Board

<img src="HardwarePortfolio/Video Balun/Video Balun PCB.jpeg" width="650">

A passive analog video transmission PCB designed as the long-distance signal interface for the system’s camera network.

The board converts single-ended composite camera signals into balanced differential pairs for transmission over twisted-pair cabling, improving noise immunity and maintaining signal integrity across long cable runs.

---

## Key Features

- Four video balun transformer channels (T1–T4)
- Converts composite video signals into differential transmission lines
- 51 Ω impedance matching on each differential output leg
- Centre-tapped secondary grounded for stable reference
- Designed for long-distance analog video transmission over twisted-pair cabling
- Integrated 2.54mm board-to-board connectors for modular system integration

---

## Design Highlights

- Passive analog front-end (no active amplification)
- Impedance-matched signal conversion for minimal reflection loss
- Differential signalling over unshielded twisted pair (UTP)
- Modular integration with breakout board via standard headers
- Designed for robustness in electrically noisy environments
- Part of a layered camera + communication system architecture

---

<img src="HardwarePortfolio/Video Balun/Video Balun Schematic.jpeg" width="650">
