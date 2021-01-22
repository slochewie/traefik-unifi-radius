# Unifi Controller, Radius, Daloradius, Mariadb and Traefik
https://hub.docker.com/r/linuxserver/unifi-controller

This is a work in progress.
End result will be a Unifi Controller with Radius/Daloradius integration and Mariadb storage.
Both Unifi Controller and Radius will be behind a Traefik reverse proxy with Let's Encrypt SSL certificates.
The final project will allow Captive Portal and WPA Enterprise WiFi freatures to be used.
Unifi controller and Daloradius will each need a dedicated URL such as unifi.example.com and radius.example.com.


Edit the docker-compose.yml as needed for your installation such as ports. If you require access from outside your local network poke holes in your router's firewall as needed.

```
mkdir -p $HOME/docker/
```
```
cd $HOME/docker/
```
```
git clone https://github.com/slochewie/unifi-radius.git
```
```
cd $HOME/docker/unifi-radius
```
```
docker-compose pull
```
```
docker-compose up -d
```
