# VisionX-OS

[![Version](https://img.shields.io/badge/version-1.1.0--stable-blue?style=flat-square)](https://github.com/VisionX/VisionX-OS)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Debian--based-D11941?style=flat-square&logo=debian)](https://www.debian.org/)
[![Security](https://img.shields.io/badge/security-verified-success?style=flat-square)](https://github.com/VisionX/VisionX-OS)

VisionX-OS is a lightweight, Debian-based Linux distribution designed specifically for individuals who want to **learn and practice cybersecurity** in a safe, structured, and accessible environment. 

Whether you are a beginner taking your first steps into networking or an intermediate user refining your penetration testing skills, VisionX-OS provides a pre-configured toolkit and a seamless learning experience right out of the box.

---

## 🌟 Project Overview

VisionX-OS bridges the gap between complex security distributions and user-friendly operating systems. Our mission is to make cybersecurity education approachable for everyone—from students and developers to IT professionals.

*   **Learning-Oriented**: Includes an integrated help system and intuitive CLI tools designed to guide you through common security workflows.
*   **Safe & Structured**: Built on the stability of Debian, providing a reliable environment for ethical hacking and defensive practice.
*   **Lightweight & Efficient**: Stripped of unnecessary bloat, VisionX-OS runs smoothly on virtual machines or older hardware.

> [!NOTE]
> VisionX-OS is intended for educational purposes and authorized security research within your own lab environments.

---

## ✨ Key Features

*   **📚 Learning Focus**: Integrated documentation and tutorials accessible directly from the terminal.
*   **🛠️ Pre-installed Tools**: A curated selection of industry-standard tools (Nmap, Metasploit, Burp Suite, etc.) ready for immediate use.
*   **🧩 Modular Design**: Tools are organized into logical modules, allowing you to install or update only what you need.
*   **🤝 Integrated Help**: Use `visionx help <tool>` to get instant, beginner-friendly guidance on how to use any pre-installed utility.
*   **🚀 Developer Ready**: Full support for Python, Go, Rust, and Node.js with pre-configured IDE environments.
*   **🛡️ Robust Security**: Built-in firewall, minimal active services, and regular automated security updates.

---

## 🔧 Tools & Modules

VisionX-OS organizes its tools into searchable modules to help you find what you need quickly. For a comprehensive catalog of all 150+ pre-installed tools, please refer to the [Tools Manifest](TOOLS.md).

### Quick Commands
```bash
# List all available security modules
visionx tools list

# Get detailed help on a specific tool (e.g., nmap)
visionx help nmap

# Search for a tool by keyword
visionx search reconnaissance
```

---

## 📂 Modules

The system is categorized into several core modules to simplify your learning journey:

| Module | Purpose | Description |
| :--- | :--- | :--- |
| **Daily Use** | Productivity | Web browsers, text editors, and essential system utilities. |
| **Developer Stack** | Development | Full compiler suites and modern IDEs (VS Code, Vim). |
| **Exploitation** | Penetration Testing | Frameworks like Metasploit and social engineering tools. |
| **Network** | Infrastructure | Scanning, mapping, and packet analysis (Nmap, Wireshark). |
| **OSINT** | Intelligence | Tools for gathering public data from various online sources. |
| **Password Cracking** | Cryptography | Industry standards such as Hashcat and John the Ripper. |
| **Reverse Engineering** | Software Analysis | Ghidra and Radare2 for analyzing binary files safely. |
| **Web Security** | Web Apps | Specialized tools for scanning and securing web applications. |
| **Wireless** | WiFi Auditing | Tools for testing the security of wireless networks. |

---

## 💾 Installation

VisionX-OS can be run as a Live ISO, installed in a Virtual Machine, or used on physical hardware.

### Minimum System Specs
*   **RAM**: 2GB (Minimum) | 4GB+ (Recommended)
*   **Storage**: 20GB free space
*   **Processor**: 64-bit capable CPU

### Getting Started
1.  **Download** the latest `.iso` file from our releases page.
2.  **Flash** to a USB drive or mount in your VM software (VirtualBox/VMware).
3.  **Update** your system once installed:

```bash
# Standard system update
sudo apt update && sudo apt upgrade -y

# VisionX specific tool sync
visionx tools update
```

---

## 🖥️ Usage

VisionX-OS provides a powerful CLI framework designed for clarity.

### Accessing the Shell
Launch the core VisionX environment to start your session:
```bash
visionx shell
```

### Automation & Pipelines
For guided reconnaissance or vulnerability assessments, use our built-in pipelines:
```bash
# Run an automated reconnaissance scan
visionx run auto-recon --target 192.168.1.10

# Execute an guided autopwn sequence (for authorized targets)
visionx run autopwn --target your-lab-target --output ./reports/
```

### Reporting
Generate professional markdown or PDF reports of your findings:
```bash
visionx report generate --session last --format pdf
```

---

## 🛡️ Security & Privacy

*   **Pre-configured Firewall**: Strict default rules to protect your system from outside traffic.
*   **Rootkit Detection**: Integrated `chkrootkit` runs periodically to ensure system integrity.
*   **Minimal Services**: Only the most essential system services are enabled by default to reduce attack surface.
*   **Encrypted Storage**: Support for full-disk encryption during the installation process.

---

## 📁 Project Structure

```text
VisionX-OS/
├── bin/                # VisionX-CLI binaries
├── core/               # System core files and configs
├── modules/            # Categorized security tools
├── scripts/            # Automation and setup scripts
├── templates/          # Standardized reporting templates
├── README.md           # This file
└── TOOLS.md            # Detailed tools manifest
```

---

## 🤝 Contributing

We welcome contributions from educators and security enthusiasts!

1.  **Fork** the repository.
2.  Create a new **Branch** (`git checkout -b feature/NewComponent`).
3.  **Commit** your changes with clear descriptions.
4.  Push to your fork and submit a **Pull Request**.

---

## 📚 Resources

*   🌐 [Official Website](https://visionx-os.org)
*   📖 [Documentation Portal](https://docs.visionx-os.org)
*   📟 [CLI Guides & Tutorials](https://visionx-os.org/cli-guide)

---

## 📜 License

VisionX-OS is released under the **MIT License**. See [LICENSE](LICENSE) for details.

---

<p align="center">
  Empowering the next generation of security professionals. <br>
  <b>Learn. Practice. Secure.</b>
</p>
