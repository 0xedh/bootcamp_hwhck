# 🔧 Hardware Hacking Bootcamp ES

Welcome to the **Hardware Hacking ES Bootcamp** @0xedh's repository!
This project provides hands-on examples, tools, and documentation to learn how to analyze, understand, and extract secrets from dTPMs.

---

## 📁 Repository Structure

```
bootcamp_hwhck/
│            
├── 1.TPM/                  # TPM analysis with tpm2tools
├── 2.VMK_hw/                  # BitLocker VMK extraction (hardware)
├── 3.VMK_sw/               # BitLocker VMK extraction (software)
├── 4.Drivers/             # Vulnerable driver analysis and kernel-mode exploitation
├── screenshots/  
├── README.md              # This file
└── references.md             # References and citations
```

---

## 📘 Documentation

All guides and exercises are written in Markdown format and located in the numerated folders.

| Guide | Description |
|-------|-------------|
| `1.TPM.md` | TPM2 operations inside Docker, key generation, sealing, and signing |
| `2.VMK_hw.md` | Extract VMK from Saleae Logic captures and mount BitLocker volumes |
| `3.VMK_sw.md` | Extract VMK with bitpixie exploit chain, modify HIVES, etc |
| `4.Drivers.md` | Analyze and exploit a vulnerable Windows kernel driver |


---

## Requirements

- **Logic2** by Saleae  
  [Download](https://www.saleae.com/downloads/) , for capturing and analyzing SPI traffic.

- **Docker**  
  Used for running TPM2 tools labs in a contained environment.

- **Dislocker**  
  Used to mount BitLocker-encrypted volumes using extracted VMK.

- **Ghidra**  
  [Download](https://ghidra-sre.org/) , for reverse engineering vulnerable drivers (binary analysis).

- **Visual Studio (Community or Pro)**  
  Recommended for compiling and debugging.

- Common Unix tools:  
  `xxd`, `grep`, `cut`, `sed`, `tr` , used for scripting and parsing exported data (CSV, hex, etc).

---

## Quick Setup

### 1. Clone the repository
```bash
git clone https://github.com/youruser/bootcamp_hwhck.git
cd bootcamp_hwhck
```
---

## Authors & Contributors

- @0xedh
- Contributions welcome! Fork this repo and submit a PR.

---

## 🛡️ Disclaimer

This repository is for **educational purposes only**.
Use of the included techniques and tools must comply with applicable laws and regulations.
Always obtain permission before testing hardware or systems you do not own.

---
