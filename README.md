# 🚀 Mars–Earth Intelligent Communication System

> **NASA Space Apps Hackathon Project**
> A hardware-software communication system simulating intelligent light-based messaging between Mars and Earth using Morse code, LEDs, and servo-mounted photoresistors.

---

## 📺 Demo

[![Demo Video](https://img.shields.io/badge/Watch%20Demo-YouTube%20Shorts-red?logo=youtube)](https://youtube.com/shorts/8LbxBmnD4wU?si=mEGBH-9Om1925tKo)

---

## 🌌 Overview

Deep space communication faces extreme challenges — radio waves take up to 24 minutes to travel between Mars and Earth. This project proposes an **optical Morse code communication system** that:

- Encodes messages as **Morse code pulses transmitted via LEDs**
- Uses **servo-mounted photoresistors** that rotate **360°** to actively scan for and lock onto the strongest light source
- Automatically decodes received light signals and prints the **original message to the terminal**

Inspired by NASA's real-world challenge of maintaining reliable communication across interplanetary distances.

---

## ⚙️ How It Works

```
[ Input Message ]
       │
       ▼
[ Morse Code Encoder ]
       │
       ▼
[ LED Array (Light Transmitter) ]
       │   (light pulses)
       ▼
[ Photoresistor on Servo Motor ]  ◄── rotates 360° to track strongest light
       │
       ▼
[ Signal Decoder ]
       │
       ▼
[ Terminal Output: Decoded Message ]
```

### Step-by-step

1. **Message Input** — The user types a text message into the system.
2. **Morse Encoding** — The message is converted into Morse code (dots and dashes).
3. **LED Transmission** — LEDs blink in Morse patterns, transmitting light pulses as the signal.
4. **Smart Light Tracking** — A photoresistor mounted on a **servo motor** continuously rotates 360° to identify and **focus on the strongest light source**, simulating a receiver satellite aligning to a transmitter.
5. **Signal Decoding** — Captured light pulses are decoded from Morse back into text.
6. **Terminal Output** — The decoded message is displayed in the terminal.

---

## 🛠️ Hardware Components

| Component | Purpose |
|---|---|
| **LEDs** | Light transmitter — blinks Morse code signals |
| **Photoresistors (LDR)** | Light receiver — detects incoming light pulses |
| **Servo Motor** | Rotates the photoresistor 360° to scan and track the strongest light source |
| **Microcontroller** | Drives the LEDs, reads sensor data, controls the servo |

---

## 💻 Software Features

- ✅ **Text → Morse Code Encoder** — Converts any text message into Morse code
- ✅ **Morse Code → Text Decoder** — Reconstructs the original message from light signals
- ✅ **Servo Control Logic** — Rotates the photoresistor to actively seek the strongest light
- ✅ **Auto Light Tracking** — Photoresistor always locks onto the brightest signal source
- ✅ **Terminal Communication Interface** — Real-time decoded message display

---

## 🚀 Getting Started

### Prerequisites

- A compatible microcontroller (e.g., Arduino / Raspberry Pi)
- Python 3.x (or Arduino IDE, depending on your stack)
- Required hardware components listed above
- Serial communication library (e.g., `pyserial` for Python)

### Installation

```bash
# Clone the repository
git clone https://github.com/BodenDuman/Hackhaton-Code-CommunicationSystem.git

# Navigate into the project directory
cd Hackhaton-Code-CommunicationSystem
```

### Running the System

```bash
# Install dependencies (if applicable)
pip install -r requirements.txt

# Run the communication system
python main.py
```

> ⚡ Make sure your hardware is connected and the correct serial port is configured before running.

---

## 🌍 Real-World Inspiration

| Challenge | Our Solution |
|---|---|
| Radio signal delay (up to 24 min) | Optical burst transmission with Morse encoding |
| Receiver alignment in space | Servo-driven 360° photoresistor auto-tracking |
| Signal noise / interference | Focus on strongest light source (highest SNR) |

---

## 🏆 Hackathon

> 🥇 **1st Place Winner!**

This project was built for the **NASA Space Apps Challenge**, a global hackathon focused on solving real space exploration problems using technology and creativity.

---

## 👥 Team

| Name | Role |
|---|---|
| **Duman Boden** | Team Member |
| **Duman Otarbyaev** | Team Member |
| **Timur Muzhikbayev** | Team Member |

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<p align="center">
  Made with ❤️ for the stars 🌠 | NASA Space Apps Hackathon
</p>
