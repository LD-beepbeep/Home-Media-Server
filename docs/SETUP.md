# Setup

This document describes the process I followed to build the server.

This is documentation of my setup rather than a guaranteed step-by-step installation guide.

---

## 1. Hardware

I started with an old laptop that was available to use as a server.

The exact hardware specifications are documented in [`HARDWARE.md`](HARDWARE.md).

---

## 2. Operating system

I installed Ubuntu/Linux (previously running Windows 7) and configured the laptop to operate as a server.

Initial configuration included:

- network configuration
- system updates
- user setup
- storage setup
- remote administration

---

## 3. Server management

Cockpit was installed to make server administration easier.

It provides a graphical interface for:

- monitoring resources
- viewing storage
- managing services
- accessing a terminal
- viewing system information

---

## 4. Media server

Jellyfin was installed as the main media server.

The media library was then configured and organised.

---

## 5. Media automation

The media-management stack was gradually expanded with services such as:

- Jellyseerr
- Sonarr
- Radarr
- Prowlarr
- qBittorrent

The services work together to automate parts of the media-management process.

---

## 6. Remote access

Tailscale was configured to allow private remote access to the server.

Private network information is not included in this repository.

---

## 7. Monitoring

Monitoring was added using:

- Uptime Kuma
- Cockpit
- Jellystat
- Watch Your LAN

Discord notifications were also configured for important events.

---

## 8. Additional services

The server was gradually expanded with:

- File Browser
- Nginx Proxy Manager
- AdGuard Home
- Home Assistant
- MeTube
- Byparr

The system grew organically as I found new problems to solve or services that were useful.

---
