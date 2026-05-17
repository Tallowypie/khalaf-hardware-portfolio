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

<img src="assets/tcu/hero.png" width="700">

A custom 4-layer communication and processing PCB designed as the upper board in a stacked two-board architecture, mounted directly above the TPU using shared standoffs.

The TCU acts as the central communication and control hub of the system, receiving power and low-level signals from the TPU while handling wireless communication, CAN networking, USB programming, and analog camera interfacing.

---

## My Role
- Full schematic capture in :contentReference[oaicite:0]{index=0}
- 4-layer PCB layout and routing
- Component selection and interface design
- Power tree design and signal integrity considerations
- Hardware debugging and bring-up

---

## Key Technical Features

### Embedded Processing
- ESP32-WROOM-32 as central MCU
- Dual UART channels
- Dual SPI buses (VSPI + HSPI)
- Relay and Hall-effect sensor control

---

### USB Programming Interface
- Dual CH340G bridges
- Independent USB Type-B interfaces
- Automatic ESP32 boot/program circuit using BC817 transistors
- Supports simultaneous monitoring/programming

---

### CAN Communication
- Dual MCP2515 + TJA1050 nodes
- Shared CAN differential bus
- 120 Ω termination
- TVS protection for transient suppression

---

### Wireless Communication
- HC-12 for long-range communication
- nRF24L01 for short-range high-speed communication
- Dual-band wireless redundancy

---

### Sensor / Camera Interfaces
- 4 analog camera channels
- Differential routing through RJ45 connectors
- Combined structured cabling for camera and CAN lines

---

### Power System
- 5V input from TPU
- AMS1117 for logic rails
- USB polyfuse protection
- Dedicated power switch

---

## Design Highlights
- 4-layer PCB stackup: Signal / GND / Power / Signal
- Controlled differential routing for CAN and camera lines
- ESD/transient protection on external interfaces
- Mechanical stack alignment with TPU using shared mounting holes

---

## PCB Layout
<img src="assets/tcu/layout.png" width="700">

---

## Key Schematic
<img src="assets/tcu/schematic.png" width="700">

---

## Final Board
<img src="assets/tcu/final_board.png" width="700">

---

# Contact
Email: your@email.com
LinkedIn: your-link
GitHub: your-link
