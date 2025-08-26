# home-lab
This homelab runs on a 256 GB Linux server using Docker and Docker Compose for container management. Services are organized with persistent storage and a single main docker-compose.yml file for easy deployment and updates.

Services running via Docker Compose

Jellyfin – self-hosted media server for movies, music, and TV shows

qBittorrent – torrent client with a web interface for remote management

Uptime Kuma – lightweight monitoring tool to keep track of service uptime

Directory structure

apps/ → persistent configuration for each service (JellyFin, qbittorrent, uptimekuma)

docker-compose.yml → central file to manage all containers

sambashare/ → shared storage for media files (Movies, Music, TV_Shows)

Downloads/ → temporary files and utilities

This setup provides a simple, maintainable way to run self-hosted services on a single machine, with clear separation of configs and data for easy backup and scaling.
