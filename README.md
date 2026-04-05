# 🔨 OChisel

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-ONetwork%20%2F%20Packet%20Crafting-red?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(stdlib)-yellow?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v1.0-cyan?style=flat-square"/>
</p>

> **OChisel** is a powerful network packet crafter for TCP, UDP, and ICMP. It allows full control over IP/TCP/UDP/ICMP headers, accurate checksum calculation, colored hex dumps, and raw packet transmission (requires root).

**Designed for advanced network testing, protocol research, and authorized red team operations.**

---

## 📌 Overview

OChisel lets you craft, inspect, decode, and transmit raw network packets with complete control over every field. It features professional colored hex dumps, flag presets, flood mode, and multiple export formats (Binary, Hex, TXT).

Perfect for protocol fuzzing, custom scanning, and low-level network experimentation.

---

## 🖥️ Modules

| # | Module               | Description |
|---|----------------------|-------------|
| **[1]** | **Craft TCP**        | Full TCP/IP packet builder with flag presets |
| **[2]** | **Craft UDP**        | UDP datagram with optional payload |
| **[3]** | **Craft ICMP**       | ICMP echo / custom type & code |
| **[4]** | **Decode Hex**       | Parse raw hex → detailed field breakdown |
| **[5]** | **Quick SYN**        | Fast SYN packet creation + optional transmit |

---

## 📊 Key Features

- **Full Packet Crafting** — TCP (with all flags), UDP, ICMP
- **Accurate Checksums** — RFC-compliant IP, TCP, UDP, ICMP checksums
- **Colored Hex Dump** — IP (orange), TCP (cyan), UDP (blue), ICMP (magenta), Payload (dim)
- **Flag Presets** — SYN, SYN-ACK, ACK, FIN-ACK, RST, XMAS, NULL, Custom
- **Transmission** — Raw socket sending (requires root)
- **Flood Mode** — High-speed packet flooding with delay control
- **Export Options**:
  - Binary (.bin) — raw bytes
  - Hex (.hex) — space-separated with metadata
  - TXT (.txt) — full human-readable report + hex dump
- **Clean Terminal UI** — Professional colored output and help system

---

## ⚙️ Requirements

- **Linux** (recommended for raw sockets)
- **Root / sudo** — Required for packet transmission
- No external Python packages (pure standard library)

**Standalone executable** — Runs as `./OChisel` when built with PyInstaller.

---

## 🚀 Usage

```bash
sudo ./OChisel

📁 Output

Live Terminal — Colored hex dump + field summary
Reports (saved in ochisel_reports/):
ochisel_YYYYMMDD_HHMMSS.bin — Raw binary packet
ochisel_YYYYMMDD_HHMMSS.hex — Hex dump with metadata
ochisel_YYYYMMDD_HHMMSS.txt — Full human-readable report



📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.
AUTHORISED NETWORK TESTING & PACKET CRAFTING USE ONLY
