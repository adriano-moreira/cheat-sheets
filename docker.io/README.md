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
