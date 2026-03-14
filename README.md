# System Dashboard

A PyQt6 desktop dashboard for monitoring my Arch Linux setup — CPU, RAM, temperatures, package updates, systemd services, and more, all in one place.

I built this because I wanted a quick-glance panel for my Hyprland setup without opening a browser or running something like an Electron app. It's been a genuinely useful side project to have running.

<img width="1920" height="1050" alt="System Dashboard screenshot" src="https://github.com/user-attachments/assets/60aac144-2dbf-4a49-a73d-7e8ac9c22453" />

---

## What it tracks

- **CPU, RAM, disk** — live usage and progress bars
- **Network I/O** — real-time rates in the header
- **Battery** — charge level and AC status
- **Hardware temps** — per-sensor readings, flashes red if critical
- **Package updates** — Pacman and AUR counts (cached, refreshed hourly)
- **Systemd health** — broken, running, or stopped services (system and user scope)
- **Kernel & journal alerts** — filterable by severity
- **Filen Cloud Sync** — sync pair status, recent logs, and account quota
- **Active network sockets** — top connected processes

---

## Getting started

1. Clone the repo:
   ```bash
   git clone https://codeberg.org/bgonc/system-dashboard.git
   cd system-dashboard
   ```

2. Set up a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run:
   ```bash
   ./run.sh
   ```

`run.sh` takes care of activating the venv and setting `QT_QPA_PLATFORM=wayland` for native rendering.

---

## Requirements

- Arch Linux (or any systemd-based distro)
- Hyprland or another Wayland compositor
- Python 3.11+
- `psutil`, `PyQt6` (see `requirements.txt`)

---

## License

GPL-3.0 — see [LICENSE](LICENSE).  
If you build on this, keep it open.

---

## Author

[Bruno Goncalves](https://bgonc.codeberg.page) · [codeberg.org/bgonc](https://codeberg.org/bgonc)
