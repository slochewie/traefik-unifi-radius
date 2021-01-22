# Unifi Controller, Radius, Daloradius, Mariadb and Traefik
https://hub.docker.com/r/linuxserver/unifi-controller

This is a work in progress.
End result will be a Docker stack containing Unifi Controller, Radius, Daloradius and Mariadb.


Both Unifi Controller and Radius will be behind a Traefik reverse proxy with Let's Encrypt SSL certificates.

Radius will allow Unifi Captive Portal and WPA Enterprise logins.

Unifi controller and Daloradius will each need a dedicated URL such as unifi.example.com and radius.example.com.




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



## Author

Aaron Wilson <https://niteowl.dev>

[![](https://cdn.buymeacoffee.com/buttons/default-blue.png)](https://www.buymeacoffee.com/slochewie)

## License

[MIT License](./LICENSE)
