# ESP32 CAN Bus Communication using TWAI (Transceiver & Receiver)

This project demonstrates CAN bus communication using two ESP32 boards via TWAI (Two-Wire Automotive Interface). The transceiver sends structured CAN messages, and the receiver listens and prints them over serial.

## 🔧 Hardware Required
- 2x ESP32 boards
- SN65HVD230 or compatible CAN transceivers
- Jumper wires
- 120Ω termination resistors

## ⚙️ Features
- Uses TWAI peripheral on ESP32 (CAN 2.0)
- Configurable message IDs, data bytes
- Real-time logging via Serial Monitor
- Lightweight and Arduino-compatible

## 📂 Files
- `TWAItransmit.ino` — Sends periodic CAN frames (ID, data)
- `TWAIreceive.ino` — Listens for CAN messages and prints details

## 🔌 Wiring
| ESP32 | CAN Transceiver |
|-------|-----------------|
| GPIO21 | RX              |
| GPIO22 | TX              |
| GND   | GND             |
| 3.3V  | VCC             |

> Ensure 120Ω termination on each end of the CAN bus.

## ▶️ Getting Started

1. Open each `.ino` in Arduino IDE
2. Select ESP32 board (e.g., DevKit V1)
3. Upload `TWAItransmit.ino` to sender, `TWAIreceive.ino` to receiver
4. Open serial monitor (115200 baud) on both boards

## 🧠 Concepts Covered
- TWAI peripheral (ESP32-specific CAN controller)
- CAN bus message format
- Serial communication & debugging
- Arduino C++ structure

## 📸 Example Output

