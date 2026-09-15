# 🧩 Services

This document contains an overview of the services running on the home server.

Private URLs and addresses are intentionally omitted from this public repository.

---

## 🎬 Media

### Jellyfin

**Purpose:** Media server and playback.

Jellyfin is the main interface I use to watch and organise my personal media library.

It provides access to:

- movies
- TV shows
- other media
- metadata
- playback
- user accounts

Website: https://jellyfin.org/

---

### Jellyseerr

**Purpose:** Media requests.

Jellyseerr provides an easy interface for requesting movies and TV shows.

The request can then be passed into the automated media-management system.

---

### Jellystat

**Purpose:** Jellyfin statistics.

Jellystat provides statistics and information about media usage.

It gives me a better overview of how the Jellyfin server is being used.

---

## 📥 Media automation

### Sonarr

**Purpose:** TV show management.

Sonarr manages TV show monitoring and works with the download system.

---

### Radarr

**Purpose:** Movie management.

Radarr manages movie monitoring and works with the download system.

---

### Prowlarr

**Purpose:** Indexer management.

Prowlarr acts as a central place to manage search/indexer providers used by the media automation tools.

---

### qBittorrent

**Purpose:** Download management.

qBittorrent is the download client used by the automated media workflow.

---

### MeTube

**Purpose:** Video downloading.

MeTube provides an interface for downloading online video and other supported media.

---

### Byparr

**Purpose:** Browser challenge support.

Byparr is used as part of the automated media workflow when browser-based challenges need to be handled.

---

## 🖥️ Server management

### Cockpit

**Purpose:** Server monitoring and administration.

Cockpit provides a web interface for managing the Linux server.

I use it to inspect:

- CPU usage
- RAM
- storage
- services
- logs
- terminal access

Website: https://cockpit-project.org/

---

### File Browser

**Purpose:** Web-based file management.

File Browser provides a simple interface for accessing and managing files stored on the server.

---

### Uptime Kuma

**Purpose:** Service monitoring.

Uptime Kuma monitors whether services are reachable.

When something goes offline, it can trigger a notification.

Website: https://uptime.kuma.pet/

---

### Nginx Proxy Manager

**Purpose:** Reverse proxy management.

Nginx Proxy Manager makes it easier to manage routes to different services.

It also allows services to be accessed using more readable hostnames rather than manually entering ports.

Website: https://nginxproxymanager.com/

---

## 🌐 Networking

### Tailscale

**Purpose:** Private remote access.

Tailscale allows me to securely access the server when I am away from home.

Website: https://tailscale.com/

---

### AdGuard Home

**Purpose:** DNS management and filtering.

AdGuard Home provides network-level DNS filtering and DNS management.

Website: https://adguard.com/en/adguard-home/overview.html

---

### Watch Your LAN

**Purpose:** LAN monitoring.

Watch Your LAN monitors devices connecting to the local network and can notify me about network activity.

---

## 🏠 Smart home

### Home Assistant

**Purpose:** Smart-home management.

Home Assistant runs on the server and provides a central interface for managing smart-home devices.

Website: https://www.home-assistant.io/

---

## 🔔 Notifications

The server uses Discord notifications for various events.

Examples include:

- media requests
- service downtime
- server problems
- monitoring alerts

Private Discord information is not included in this repository.
