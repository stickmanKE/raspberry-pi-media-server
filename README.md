# Raspberry Pi Media Server

This project is a complete self-hosted media server setup using a Raspberry Pi. It uses Docker and Docker Compose to run various services like torrent clients, media organizers, and streaming platforms — all optimized for low power consumption and 24/7 operation.

## 🧰 Features

- **qBittorrent** – Torrent downloader with a sleek web interface
- **Sonarr** – TV series management and automatic downloading
- **Radarr** – Movie management and automation
- **Jellyfin / Plex** – Stream media across your devices
- **Homepage Dashboard** – Custom dashboard for managing services
- **Tailscale / Headscale** – Secure remote access
- **[Add your tools here]**

## 📦 Hardware Requirements

- Raspberry Pi 4 (2GB/4GB/8GB)
- microSD card (16GB minimum, 32GB+ recommended)
- External HDD or SSD (for media storage)
- Active cooling (optional but recommended)

## ⚙️ Software Stack

- Docker
- Docker Compose
- Portainer (optional)
- Pi OS Lite (recommended)

## 🚀 Setup Instructions

### 1. Flash OS and Prepare Raspberry Pi

```bash
# Update system
sudo apt update && sudo apt upgrade -y

# Install Docker & Docker Compose
curl -sSL https://get.docker.com | sh
sudo usermod -aG docker $USER


# (Optional) Reboot the Pi
sudo reboot
