## Initial work:

### Network Setup:

```docker network create --driver=bridge --subnet=10.0.0.0/8 --gateway=10.0.0.1 --attachable internalized```

### Portainer
```docker run -d -p 8000:8000 -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce```


### CaddyFile
```wget -O ~/Docker/Containers/AppData/c/caddy2plus/sites/Caddyfile https://raw.githubusercontent.com/BiosPlus/PiracyServer/main/Caddyfile/Caddyfile```
