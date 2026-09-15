# Home Media Server

A self-hosted home media and services server running on an old laptop, built and maintained by me (Lars).

The project started as a way to create a personal media library and gradually grew into a larger home lab containing media management, monitoring, networking, file management, automation and smart-home services.

> **Status:** Running and continuously improving  
> **Hardware:** Laptop  
> **Storage:** 2 TB  
> **Operating system:** Ubuntu/Linux

---

## What is this?

It runs a collection of self-hosted services that I use for:

- 🎬 watching and organising media
- 📥 managing media downloads
- 📁 storing and accessing files
- 📊 monitoring the server
- 🌐 managing parts of my network
- 🔐 accessing services remotely
- 🏠 managing smart-home devices
- 🔔 sending notifications when something goes wrong

---

## Hardware

The server currently runs on a laptop with **2 TB of storage**.

The exact hardware specifications are documented in [`docs/HARDWARE.md`](docs/HARDWARE.md).

Running a server on a laptop creates some interesting challenges around:

- power management
- cooling
- storage
- reliability
- network connectivity
- long-term operation
- and more yet to come probably :)

---

## Services

The server currently runs a large collection of services.

See [`docs/SERVICES.md`](docs/SERVICES.md) for the complete list and what each service does.

The main parts of the system are:

### Media

- Jellyfin
- Jellyseerr
- Jellystat

### Media automation

- Sonarr
- Radarr
- Prowlarr
- qBittorrent
- MeTube
- Byparr

### Server management

- Cockpit
- File Browser
- Uptime Kuma
- Nginx Proxy Manager

### Networking

- Tailscale
- AdGuard Home
- Watch Your LAN

### Smart home

- Home Assistant

### Notifications

- Discord notifications for requests and server events

---

## 🗺️ Architecture

A simplified overview of the system:

```text
                    ┌────────────────────┐
                    │    Home devices    │
                    │ PC / TV / Phone    │
                    └─────────┬──────────┘
                              │
                              ▼
                    ┌────────────────────┐
                    │    Home network    │
                    └─────────┬──────────┘
                              │
                              ▼
                    ┌────────────────────┐
                    │   Ubuntu laptop    │
                    │    Home server     │
                    └─────────┬──────────┘
                              │
       ┌──────────────────────┼──────────────────────┐
       │                      │                      │
       ▼                      ▼                      ▼
┌──────────────┐      ┌──────────────┐      ┌──────────────┐
│    Media     │      │  Management  │      │  Networking  │
│   Jellyfin   │      │   Cockpit    │      │  Tailscale   │
│ Jellyseerr   │      │ Uptime Kuma  │      │ AdGuard Home │
│  Jellystat   │      │ File Browser │      │ Watch LAN    │
└──────────────┘      └──────────────┘      └──────────────┘
       │
       ▼
┌──────────────────────────────┐
│     Media automation         │
│ Sonarr / Radarr / Prowlarr  │
│       qBittorrent            │
└──────────────────────────────┘
