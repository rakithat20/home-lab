# 🏠 Home Lab -- Always Evolving 🚀

This homelab runs on a **256 GB Linux server** using **Docker** and
**Docker Compose** for container management.\
Everything is organized with **persistent storage** and a single main
`docker-compose.yml` file for smooth deployment and updates.\
_It's a work in progress --- continuously improving, tweaking, and
adding new services!_ 🔧✨

---

## **⚡ Services running via Docker Compose**

- 🎬 **Jellyfin** -- self-hosted media server for movies, music, and
  TV shows\
- 🌊 **qBittorrent** -- torrent client with a clean web interface for
  remote management\
- 📈 **Uptime Kuma** -- lightweight monitoring to keep an eye on
  service health\
- 📺 **Sonarr** -- automated TV series management and downloading\
- 🎥 **Radarr** -- automated movie management and downloading\
- 🔎 **Prowlarr** -- indexer manager for Sonarr, Radarr, and other
  download apps

---

## **🚀 Quick Setup**

1. **Clone the repository**:

   ```bash
   git clone https://github.com/rakithat20/home-lab.git
   cd home-lab
   ```

2. **Configure environment variables**:

   ```bash
   cp .env.example .env
   ```

   Edit `.env` and update:

   - User/Group IDs (run `id` command to get your values)
   - Timezone (default: `Asia/Colombo`)
   - Ports (if needed)

3. **Start services**:
   ```bash
   docker-compose up -d
   ```

## **📂 Directory Structure**

After first run, the following structure will be created:

```
home-lab/
├── docker-compose.yml     → main container configuration
├── .env                  → your environment variables
├── data/                 → persistent app configurations
│   ├── jellyfin/
│   ├── qbittorrent/
│   ├── sonarr/
│   ├── radarr/
│   ├── prowlarr/
│   └── uptimekuma/
└── media/                → your media files
    ├── movies/
    └── tv/
```

---

## **🌐 Access Your Services**

Once running, access services at:

- **Jellyfin**: `http://localhost:8096`
- **qBittorrent**: `http://localhost:8080`
- **Sonarr**: `http://localhost:8989`
- **Radarr**: `http://localhost:7878`
- **Prowlarr**: `http://localhost:9696`
- **Uptime Kuma**: `http://localhost:3001`

_(Ports can be customized in your `.env` file)_

---

## **Why this setup?**

This homelab is designed to be:\

- **Simple** → one compose file to rule them all 🗂️\
- **Maintainable** → clear data separation for easy backup\
- **Scalable** → ready to grow with new services as I experiment 🌱
