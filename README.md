# System Dashboard

A PyQt6 desktop dashboard for Arch Linux, built for Hyprland / Wayland.  
This is a personal utility and learning project for my own daily setup.

<img width="1920" height="1050" alt="System Dashboard screenshot" src="https://github.com/user-attachments/assets/60aac144-2dbf-4a49-a73d-7e8ac9c22453" />

---

## What it monitors

- **System metrics**: CPU, RAM, disk usage, network I/O, battery
- **Hardware temperatures**: per-sensor readings
- **Network sockets**: open connections in real time
- **Package updates**: Pacman and AUR update counts (cached)
- **Systemd health**: broken, stopped, or crashed services in system and user scope
- **Kernel & journal alerts**
- **Filen Cloud Sync**: passive monitoring of sync state

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://codeberg.org/bgonc/system-dashboard.git
   cd system-dashboard
   ```

2. Create and activate a Python virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

```bash
./run.sh
```

This activates the virtual environment and sets `QT_QPA_PLATFORM=wayland` for native Wayland rendering.

---

## Requirements

- Arch Linux (or any systemd-based distro)
- Hyprland or another Wayland compositor
- Python 3.11+
- Dependencies: `psutil`, `PyQt6` (see `requirements.txt`)

---

## Usage and permission

This repository is source-available, but not open source.
Personal viewing and reference are allowed.
Reuse, modification, redistribution, derivative works, and commercial use are not permitted without prior written permission.
See [LICENSE](LICENSE) for details.

---

## Author

[Bruno Goncalves](https://bgonc.codeberg.page) · [codeberg.org/bgonc](https://codeberg.org/bgonc)
