install on Ubuntu 18.04

```
sudo apt install docker.io
sudo usermod -aG docker $USER
```

copy image over shh
```
docker save [image_name] | ssh -C [host] docker load
```
