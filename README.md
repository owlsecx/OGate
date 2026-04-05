# 🔑 OGate

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-ORec%20%2F%20Credential%20Testing-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-impacket-yellow?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v1.0-cyan?style=flat-square"/>
</p>

> **OGate** is an authorised NTLM credential validation tool that safely tests usernames and passwords against SMB (445), WinRM (5985), and RDP (3389) on Windows targets.

**Live stats, threading, OS fingerprinting, and TXT report export.**

---

## 📌 Overview

OGate validates NTLM credentials on authorised Windows systems using multiple protocols. It supports wordlist attacks, single credential testing, and quick target reconnaissance (port scan + SMB OS fingerprint).

Designed for authorised penetration testing and red team operations.

---

## 🖥️ Modules

| # | Module                  | Description |
|---|-------------------------|-------------|
| **[1]** | **Credential Validate** | Full wordlist or single password attack |
| **[2]** | **Quick Check**         | Test one username:password pair |
| **[3]** | **Target Recon**        | Port scan + SMB OS fingerprint |

---

## 📊 Key Features

- **Multi-Protocol Support** — SMB (impacket), WinRM (pywinrm), RDP (connectivity check)
- **Threaded Wordlist Attack** — Configurable threads and delay
- **Live Progress** — Real-time stats with found/failed counters
- **SMB OS Fingerprint** — Quick banner grab for OS version hint
- **Detailed Reporting** — TXT export with full session log
- **Safety First** — Strict authorisation disclaimer + safe checks

---

## ⚙️ Requirements

- **impacket** (required for SMB)
  ```bash
  pip install impacket
  pip install pywinrm
  chmod +x OGate

  📁 Output

Live Terminal — Real-time progress with found/failed counters
Summary — Tried, failed, found, elapsed time
Report File (in ogate_reports/):
ogate_<timestamp>.txt — Full session details including valid credentials



📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.
AUTHORISED SECURITY TESTING USE ONLY
