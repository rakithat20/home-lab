# 🏠 Home Lab -- Always Evolving 🚀

This homelab runs on a **256 GB Linux server** using **Docker** and
**Docker Compose** for container management.\
Everything is organized with **persistent storage** and a single main
`docker-compose.yml` file for smooth deployment and updates.\
*It's a work in progress --- continuously improving, tweaking, and
adding new services!* 🔧✨

------------------------------------------------------------------------

## **⚡ Services running via Docker Compose**

-   🎬 **Jellyfin** -- self-hosted media server for movies, music, and
    TV shows\
-   🌊 **qBittorrent** -- torrent client with a clean web interface for
    remote management\
-   📈 **Uptime Kuma** -- lightweight monitoring to keep an eye on
    service health\
-   📺 **Sonarr** -- automated TV series management and downloading\
-   🎥 **Radarr** -- automated movie management and downloading\
-   🔎 **Prowlarr** -- indexer manager for Sonarr, Radarr, and other
    download apps

------------------------------------------------------------------------

## **📂 Directory Structure**

-   **`apps/`** → persistent configuration for each service (`JellyFin`,
    `qBittorrent`, `uptimekuma`, `sonarr`, `radarr`, `prowlarr`)\
-   **`home-lab/docker-compose.yml`** → central file to manage all
    containers\
-   **`home-lab/README.md`** → documentation for the homelab\
-   **`sambashare/`** → shared storage for media files (`Movies`,
    `Music`, `TV_Shows`)\
-   **`Downloads/`** → temporary files and utilities

------------------------------------------------------------------------

## **Why this setup?**

This homelab is designed to be:\
- **Simple** → one compose file to rule them all 🗂️\
- **Maintainable** → clear data separation for easy backup\
- **Scalable** → ready to grow with new services as I experiment 🌱
