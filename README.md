# 🌌 VisionX-OS

[![Version](https://img.shields.io/badge/version-1.0.0--stable-bluegrey?style=for-the-badge&logo=linux)](https://github.com/VisionX/VisionX-OS)
[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Debian--based-D11941?style=for-the-badge&logo=debian)](https://www.debian.org/)
[![Security](https://img.shields.io/badge/security-hardened-success?style=for-the-badge&logo=securityscorecard)](https://github.com/VisionX/VisionX-OS)

```text
  _   __ _      _               _  __      ____   _____ 
 | | / /(_)____(_)___  _ __    | |/ /     / __ \ / ___/ 
 | |/ / / / ___/ / __ \| '_ \   |   /     / / / / \__ \  
 |   / / (__  / / /_/ /| | | | /   |     / /_/ / ___/ /  
 |_|/_/ \___//_/\____/ |_| |_|/_/|_|     \____/ /____/   
                                                         
  >> THE ULTIMATE LIGHTWEIGHT PENETRATION TESTING DISTRO <<
```

## ⚡ Overview

**VisionX-OS** is a specialized, lightweight Linux distribution built on the stable foundation of **Debian**. Engineered for cybersecurity professionals, penetration testers, and security-focused developers, VisionX-OS strips away the bloat to provide a blazing-fast, modular, and weaponized environment.

Whether you're performing reconnaissance, exploitation, or rapid software development, VisionX-OS provides the precision tools you need without the overhead.

> [!IMPORTANT]
> VisionX-OS is intended for educational purposes and authorized security testing only.

---

## 🚀 Key Features

*   **⚡ Lightweight Core**: Optimized kernel and minimal background services for maximum performance on any hardware.
*   **🔒 Hardened Security**: Integrated firewall, rootkit detection (`chkrootkit`), and encrypted-by-default configurations.
*   **💻 Developer-Ready**: Pre-configured with Python, Go, Rust, and Node.js environments.
*   **🖥️ Modular Toolset**: Install only what you need. Our custom module system keeps your storage lean.
*   **🛡️ Integrated Help**: A unified command-line help system for every pre-installed binary.
*   **🎭 Stealth Mode**: MAC address randomization and VPN kill-switch integration out of the box.

---

## 🛠️ Tools

VisionX-OS comes with a curated selection of industry-standard tools. To keep this README clean, please refer to the full catalog in our tools manifest:

👉 **[View Full Tool Catalog (TOOLS.md)](TOOLS.md)**

### Quick Commands
```bash
# List all installed security modules
visionx tools list

# Get deep-dive help on a specific tool
visionx help nmap

# Update the VisionX tool repository
visionx tools update --force
```

---

## 📦 Installation

### Recommended Specs
*   **RAM**: 2GB (Minimum) | 8GB (Recommended)
*   **Storage**: 20GB SSD
*   **OS**: Debian 12 (Core Base)

### Setup & Initialization
Clone the repository and run the setup script:

```bash
git clone https://github.com/VisionX/VisionX-OS.git
cd VisionX-OS
sudo chmod +x setup.sh
./setup.sh --install-core
```

Update your system to the latest VisionX patches:
```bash
sudo apt update && sudo apt full-upgrade -y
visionx upgrade
```

---

## 🎮 Usage

### Launching the Framework
The `visionx` CLI is the heartbeat of the OS.

```bash
# Start the global shell module
visionx shell
```

### Autopwn Pipeline (Experimental)
Run an automated vulnerability scanning and reporting pipeline:

```bash
visionx run autopwn --target 192.168.1.1/24 --output ./reports/
```

### Report Generation
Export your findings into professional JSON or PDF formats:

```bash
visionx report generate --session last_scan --format pdf
```

---

## 🧩 Modules

VisionX-OS is organized into logical modules. You can enable/disable these to suit your mission:

| Module | Description | Icon |
| :--- | :--- | :--- |
| **Daily Use** | Essential apps for productivity and browsing. | 🏢 |
| **Developer Stack** | Compilers, IDEs (VS Code/Vim), and git tools. | 🛠️ |
| **Exploitation** | Metasploit, BeEF, and custom exploits. | 💣 |
| **Network** | Nmap, Wireshark, ZMap, and scanning utilities. | 🌐 |
| **OSINT** | Maltego, SpiderFoot, and social scrapers. | 🔍 |
| **Password Cracking**| Hashcat, John the Ripper, and wordlists. | 🔑 |
| **Reverse Engineering**| Ghidra, Cutter, and GDB. | 🧬 |
| **Web Security** | Burp Suite, SQLMap, and Nikto. | 🕸️ |
| **Wireless** | Aircrack-ng, Kismet, and Wifite. | 📡 |

---

## 🛡️ Security & Privacy

*   **UFW Pre-configured**: Strict inbound rules by default.
*   **Micro-Services**: Only essential ports (SSH/Internal) are open.
*   **Live Rootkit Scanning**: Daily `rkhunter` checks.
*   **Zero Logs (Optional)**: Enable "Privacy Mode" to prevent local command history and log persistence.

---

## 📂 Project Structure

```text
VisionX-OS/
├── bin/                # Core VisionX binaries
├── configs/            # System & Shell configurations
├── docs/               # Manuals and API docs
├── modules/            # Searchable tool modules
│   ├── exploitation/
│   ├── network/
│   └── osint/
├── scripts/            # Automation & Setup scripts
├── templates/          # Report & Project templates
├── README.md           # You are here
└── TOOLS.md            # Full tool documentation
```

---

## 🤝 Contribution

We welcome contributions from the community!

1.  **Fork** the project.
2.  Create your **Feature Branch** (`git checkout -b feature/AmazingFeature`).
3.  **Commit** your changes (`git commit -m 'Add some AmazingFeature'`).
4.  **Push** to the branch (`git push origin feature/AmazingFeature`).
5.  Open a **Pull Request**.

---

## 📚 Resources

*   🌐 [Official Website](https://visionx-os.com)
*   📖 [Documentation Portal](https://docs.visionx-os.com)
*   📺 [CLI Usage Tutorials](https://youtube.com/visionx-os)

---

## 📜 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

<p align="center">
  Generated with 💜 by the VisionX Community. <br>
  Built for <b>Freedom</b>. Built for <b>Security</b>.
</p>
