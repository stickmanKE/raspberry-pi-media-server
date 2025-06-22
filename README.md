# Raspberry Pi Media Server

A simple, lightweight, and ARM-friendly Docker-based media server stack built for Raspberry Pi.
## 🧰 Features

- **qBittorrent** – Torrent downloader with a sleek web interface
- **Sonarr** – TV series management and automatic downloading
- **Radarr** – Movie management and automation
- **Jellyfin / Plex** – Stream media across your devices
- **Homepage Dashboard** – Custom dashboard for managing services
- **Tailscale / Headscale** – Secure remote access

## 📷 Screenshot

![Media Dashboard Screenshot](assets/homepage.png) 

## 🧰 Included Services

| Service     | Purpose                        | Port |
|-------------|--------------------------------|------|
| Homepage    | Dashboard UI                   | 3000 |
| qBittorrent | Torrent Client + VueTorrent UI | 8080 |
| Sonarr      | TV Show Management             | 8989 |
| Radarr      | Movie Management               | 7878 |
| Jackett     | Indexer Proxy for Torrent Sites| 9117 |
| Pi-hole     | Network-wide Ad Blocking       | 80/53/443 |

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
