# 🏠 Home Lab – Always Evolving 🚀  

This homelab runs on a **256 GB Linux server** using **Docker** and **Docker Compose** for container management.  
Everything is organized with **persistent storage** and a single main `docker-compose.yml` file for smooth deployment and updates.  
_It's a work in progress — continuously improving, tweaking, and adding new services!_ 🔧✨  

---

## **⚡ Services running via Docker Compose**
- 🎬 **Jellyfin** – self-hosted media server for movies, music, and TV shows  
- 🌊 **qBittorrent** – torrent client with a clean web interface for remote management  
- 📈 **Uptime Kuma** – lightweight monitoring to keep an eye on service health  

---

## **📂 Directory Structure**
- **`apps/`** → persistent configuration for each service (`JellyFin`, `qbittorrent`, `uptimekuma`)  
- **`docker-compose.yml`** → central file to manage all containers  
- **`sambashare/`** → shared storage for media files (`Movies`, `Music`, `TV_Shows`)  
- **`Downloads/`** → temporary files and utilities  

---

## **Why this setup?**  
This homelab is designed to be:  
- **Simple** → one compose file to rule them all 🗂️  
- **Maintainable** → clear data separation for easy backup  
- **Scalable** → ready to grow with new services as I experiment 🌱  
