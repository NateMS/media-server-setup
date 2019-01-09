# Media Server Setup

Description of the setup I use for my media server.
I have a Drobo attached directly, so I am using that as storage for all of my media.

**OS**
Windows Server 2019

**Applications**
Install the following applications:

- [Git](https://git-scm.com/download/win)
- [Docker](https://www.docker.com/products/docker-desktop)
- [Docker-Compose](https://docs.docker.com/docker-for-windows/install/)
- [Drobo Dashboard](https://www.drobo.com/docs/start-5d/)

## Setting up Docker

I am using the following docker images to run these applications inside a container:

- *[linuxserver/plex](https://hub.docker.com/r/linuxserver/plex/)* - Plex Media Server
- *[linuxserver/tautulli](https://hub.docker.com/r/linuxserver/tautulli)* - Monitoring, analytics and notifications for Plex Media Server
- *[linuxserver/radarr](https://hub.docker.com/r/linuxserver/radarr)* - Monitoring and tracking Movies
- *[linuxserver/sonarr](https://hub.docker.com/r/linuxserver/sonarr)* - Monitoring and tracking TV-Shows
- *[linuxserver/bazarr](https://hub.docker.com/r/linuxserver/bazarr)* - Monitoring and tracking Subtitles
- *[linuxserver/jackett](https://hub.docker.com/r/linuxserver/jackett)* - API Support for various trackers
- *[linuxserver/ombi](https://hub.docker.com/r/linuxserver/ombi)* - Plex Request and user management system
- *[haugene/transmission-openvpn](https://github.com/haugene/docker-transmission-openvpn)* - Torrent Client with VPN
- *[portainer/portainer](https://hub.docker.com/r/portainer/portainer)* - GUI for managing Docker
- *[v2tec/watchtower](https://hub.docker.com/r/v2tec/watchtower)* - Automatically restart containers when base image is refreshed
- *[lsiocommunity/organizr](https://hub.docker.com/r/lsiocommunity/organizr/)* - Show all Docker Services in one place

The configurations for the docker images are saved in the docker-compose.yaml file.