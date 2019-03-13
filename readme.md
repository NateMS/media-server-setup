# Media Server Setup

Description of the setup I use for my media server.

## Setting up Docker

I am using the following docker images to run these applications inside a container:

- *[linuxserver/tautulli](https://hub.docker.com/r/linuxserver/tautulli)* - Monitoring, analytics and notifications for Plex Media Server
- *[linuxserver/radarr](https://hub.docker.com/r/linuxserver/radarr)* - Monitoring and tracking Movies
- *[linuxserver/sonarr](https://hub.docker.com/r/linuxserver/sonarr)* - Monitoring and tracking TV-Shows
- *[linuxserver/lidarr](https://hub.docker.com/r/linuxserver/lidarr)* - Monitoring and tracking Music
- *[linuxserver/bazarr](https://hub.docker.com/r/linuxserver/bazarr)* - Monitoring and tracking Subtitles
- *[linuxserver/calibre-web](https://hub.docker.com/r/linuxserver/calibre-web)* - Managing and organizing e-books
- *[thraxis/lazylibrarian-calibre](https://hub.docker.com/r/linuxserver/thraxis/lazylibrarian-calibre)* - Monitoring and tracking e-books, magazines, comics and audiobooks
- *[linuxserver/jackett](https://hub.docker.com/r/linuxserver/jackett)* - API Support for various trackers
- *[linuxserver/ombi](https://hub.docker.com/r/linuxserver/ombi)* - Plex Request and user management system
- *[binhex/arch-rtorrentvpn](https://hub.docker.com/r/binhex/arch-rtorrentvpn)* - Torrent Client with VPN
- *[portainer/portainer](https://hub.docker.com/r/portainer/portainer)* - GUI for managing Docker
- *[v2tec/watchtower](https://hub.docker.com/r/v2tec/watchtower)* - Automatically restart containers when base image is refreshed
- *[linuxserver/heimdall](https://hub.docker.com/r/linuxserver/heimdall)* - neat overview page

The configurations for the docker images are saved in the docker-compose.yml file.
In the same directory as the docker file, there needs to be a .env file to supply the necessary variables.