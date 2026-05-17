# Ahmed Khalaf
## Hardware / Robotics Engineer

---

# Projects

---

## Topside Communication Unit (TCU)

<img src="HardwarePortfolio/Topside Control Unit/TCU ASSEMBLY.png" width="400">

A 2-layer communication hub designed as part of a custom ROV electronics stack. Integrates an ESP32 with dual CAN bus nodes, dual CH340G USB-to-UART bridges with an auto-programmer circuit, HC-12 and nRF24L01 dual-band wireless, and four analog camera channels — all on a single board that stacks directly above the TPU on shared standoffs.

### Key Features
- ESP32-WROOM-32 main controller  
- Dual CH340G USB interfaces  
- Dual CAN bus nodes (MCP2515 + TJA1050)  
- HC-12 + nRF24L01 wireless communication  
- 4x analog camera inputs via RJ45  
- Regulated 3.3V logic power with protection  

<img src="HardwarePortfolio/Topside Control Unit/TCU PCB.png" width="400">

---

## Topside Power Unit (TPU)

<img src="HardwarePortfolio/Topside Power Unit/TPU PCB.png" width="400">

The power foundation of the ROV topside stack, managing dual 48V and 12V input rails with polyfuse protection, varistor clamping, ACS712 Hall-effect current sensing up to ±30A, and a relay-switched 48V output driven through an optocoupler for galvanic isolation.

### Key Features
- 48V + 12V dual input with protection  
- ACS712 current sensing (±30A)  
- Relay-switched isolated high-voltage output  
- AMS1117 low-voltage regulation  
- Multi-rail power distribution (12V / 5V / 3.3V)  
- USB power outputs for subsystems  

<img src="HardwarePortfolio/Topside Power Unit/TPU SCHEMATIC.png" width="400">

---

## Video & Signal Breakout Board

<img src="HardwarePortfolio/Camera Board/Camera Board PCB.jpeg" width="400">

A passive 2-layer routing board that consolidates analog camera inputs, IP camera signals, and communication lines into a single structured patch point. Twelve solder jumpers allow per-channel video balun bypass without any board rework, making it practical for field debugging.

### Key Features
- 4x analog camera channels  
- Modular connector breakout system  
- Solder-jumper configurable routing  
- Separation of video and communication lines  
- System-level debugging interface  

<img src="HardwarePortfolio/Camera Board/Camera Board Schematic.jpeg" width="400">

---

## Video Balun Board

<img src="HardwarePortfolio/Video Balun/Video Balun PCB.jpeg" width="400">

Four independent transformer-based balun channels convert single-ended composite video signals into impedance-matched differential pairs for transmission over unshielded twisted-pair tether cabling, with 51Ω termination on each output leg to minimise reflections.

### Key Features
- 4x video balun transformer channels  
- 51Ω impedance matching  
- Differential transmission over UTP  
- Ground-referenced center tap design  
- Modular integration with system breakout board  

<img src="HardwarePortfolio/Video Balun/Video Balun Schematic.jpeg" width="400">

---
