install on Ubuntu 18.04

```sh
#sudo apt install docker.io
curl -sSL https://get.docker.com | sudo sh
sudo usermod -aG docker $USER
```

copy image over shh
```
docker save [image_name] | ssh -C [host] docker load
```

hoster https://hub.docker.com/r/dvdarias/docker-hoster
```
docker run --rm -d \
    -v /var/run/docker.sock:/tmp/docker.sock \
    -v /etc/hosts:/tmp/hosts \
    --name docker-hoster \
    dvdarias/docker-hoster
```
