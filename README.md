# 🏡 Homelab Configuration

This repository houses the configuration files and `docker compose` stacks for my self-hosted services and homelab infrastructure.

![Homelab Dashboard Screenshot](images/dashboard.png)

---

> [!NOTE]
> This is the setup for my media server, and you will need to adjust for your own environment, don't just blindly copy and paste.

> [!IMPORTANT]
> ProtonVPN and Caddy is used for external access, adjust your set up as needed.

---

## 💡 Concept
The primary motivations behind this structured configuration repository are:

1.  **Portability:** The use of `docker compose` ensures that the entire stack can be moved to a new machine or cloud provider with minimal changes, promoting resilience and easy hardware upgrades.
2.  **Configuration Management:** By keeping environment variables, network settings, and persistent volumes defined in declarative files, the system state is always known and version-controlled.
3.  **Reproducibility:** Every service can be deployed consistently, allowing quick restoration after a failure (the "infrastructure as code" principle).
4.  **Open Sharing:** To share the setup with the community, allowing others to learn from, adapt, and improve the configuration patterns used for a reliable homelab environment.

---

## 🛠️ Software Stack

> This is the current software stack that I currently use. 

### 🖥️ OS & Infrastructure
| Software | Purpose |
| :--- | :--- |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/proxmox.png" width="20"> [Proxmox](https://www.proxmox.com/en/) | Hypervisor / Virtualization Platform |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/portainer.png" width="20"> [Portainer](https://www.portainer.io/) | Container Management |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/cockpit.png" width="20"> [Cockpit](https://cockpit-project.org/) | Fileserver & Web-based Server Manager |
| <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/png/technitium.png" width="20"> [Technitium](https://technitium.com/dns/) | Self-hosted DNS Server |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/caddy.png" width="20"> [Caddy](https://caddyserver.com/) | Reverse Proxy with Automatic SSL |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/glances.png" width="20"> [Glances](https://github.com/nicolargo/glances) | Real-time System Monitoring |
| <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/png/speedtest-tracker.png" width="20"> [Speedtest Tracker](https://docs.speedtest-tracker.dev/) | Network Performance Tracking |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/homepage.png" width="20"> [Homepage](https://gethomepage.dev/) | Dashboard for Services |

### 🎥 Media Managment

| Software | Purpose |
| :--- | :--- |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/jellyfin.png" width="20"> [Jellyfin](https://jellyfin.org/) | Open Source Media Server |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/overseerr.png" width="20"> [Seerr](https://seerr.dev/) | Media Request & Discovery |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/radarr.png" width="20"> [Radarr](https://radarr.video/) | Movie Management |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/sonarr.png" width="20"> [Sonarr](https://sonarr.tv/) | TV Show Management |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/prowlarr.png" width="20"> [Prowlarr](https://prowlarr.com/) | Indexer Manager |
| <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/png/recyclarr.png" width="20"> [Recylarr](https://recyclarr.dev/) | Custom Profile Manager |

### 📥 Downloaders

| Software | Purpose |
| :--- | :--- |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/sabnzbd.png" width="20"> [SABnzbd](https://sabnzbd.org/) | Binary Newsgroup Downloader |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/qbittorrent.png" width="20"> [qBittorrent](https://www.qbittorrent.org/) | BitTorrent Client |

### 🔍 Download Optimizers

| Software | Purpose |
| :--- | :--- |
| <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/png/huntarr.png" width="20"> [Huntarr](https://github.com/plexguide/Huntarr.io) | Smart Content Discovery |
| <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/png/cleanuperr.png" width="20"> [Cleanuparr](https://cleanuparr.github.io/Cleanuparr/) | Downloader Cleanup Tool |

### Photos 📷

| Software | Purpose |
| :--- | :--- |
| <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/immich.png" width="20"> [Immich](https://immich.app/) | High-performance Photo/Video Backup |

---
