# 🦉 OChisel

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-ONetwork-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OChisel** — Advanced Network Packet Crafter

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OChisel is an advanced network packet crafter for authorised testing that builds, inspects, decodes, replays and captures raw TCP/UDP/ICMP/ARP/IPv6 packets. It computes accurate checksums, renders coloured hex dumps and supports PCAP export as well as import and replay. Additional modes include a port scanner, packet sniffer, protocol fuzzer and flood engine, using only the standard library.

---

## ✨ Features

- Craft raw TCP/UDP/ICMP/ARP/IPv6 packets with accurate checksums
- Decode packets from hex or .bin/.pcap files with coloured hex dump
- PCAP export plus import and replay
- TCP port scanner and live packet sniffer with filters
- Protocol fuzzer and flood engine
- No external dependencies — standard library only (root required to transmit)

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OChisel scan --src 192.168.1.5 --dst 192.168.1.10 --ports common
./OChisel craft --proto tcp --src 10.0.0.1 --dst 10.0.0.2 --dport 80
./OChisel decode --hex 450000280001...
./OChisel --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled.s.Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
